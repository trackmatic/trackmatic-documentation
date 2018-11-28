# Integration Api

The integration API provides a way to upload the complex route structure in a normalized format. There are many moving parts to a route and care should be taken when building an integration to ensure a reliable and robust result.

Each message represents a single route along with all of its associated data. Once initial validation has been performed on the message the route is dispatched asynchronously to be processed by the server. This means that the route may not be available immediately after a 200 response code is received. A web hook can be registered to notify you once the upload is complete.

This section is intended to provide the details on the technical aspects of the API. For business domain related information please read [loads in context](../)

## Open Api Documentation
For more information on available calls and messages structure [goto the open api docs](./open-api)

## Validation

The message you construct and send goes through a series of validation steps. The first phase does basic type checking and ensures that required fields have been provide. The next phase checks the referential integrity of the message. Lookup data is scanned for duplicates and lookup references are checked for consistency. If any failures are detected the API will respond with a "400 Bad Request" http status code. Details of the failure will be contained in the response message.

## Data Ownership

The data ownership component of the message is an important mechanism providing control over the ownership of various elements of the message. Using the data ownership component you are able to configure the behavior of the API for create, update and delete operations of the supported areas. The options for the operations are as follows:

- Accept - This will instruct the API to accept changes sent within the message and overwrite any data which already exists in the Trackmatic system. Using this option makes your system the owner of the data area.

- Throw Error - This option will instruct the api to throw an error if the operation is attempted. This is useful when debugging or if you are not certain of the effect that the message will have on the data.

- Ignore - When using this option the api will ignore any data sent by you if the data already exists in Trackmatic. This effectively makes Trackmatic the owner of the data area since once a component is created any further changes made by this api call will be ignored. This is useful for when you need to allow changes to me made through the Trackmatic user interface and not have them overwritten by the integration.

## Integration Keys

The integration key properties are intended to represent either your business keys or composite business keys which you create and own. This is useful for performing updates since you will not be required to call our API to retrieve the trackmatic id, instead you simply send the message again. If the integration keys matches data which has been previously uploaded an update will be performed. If an integration key does not exist in the Trackmatic system a create will be performed.

Integration keys are mapped to Trackmatic id's internally. When working with non integration apis or the Trackamtic web interface you will be working with trackmatic id's.

When webhooks are created the integration keys are retrieved and integration keys are inserted into the webhook payload so that you can correlate the webhook data with your line of business systems.

### Normalization

The payload allows you to upload supporting data in a normalized fashion. Each component can be defined once then referenced in other parts of the message using their integration keys. For example

```

  "locations": [
    {
      "integration_key": "location1"
    }
  ],

  "shipping_addresses": [
    {
      "integration_key": "shippingAddress1",
      "location_integration_key": "location1"

      ...
    }
  ],
  "entities": [
    {
      "integration_key": "entity1"

      ...
    }
  ],
  "consignments": [
    {
      "integration_key": "consignment1",
      "dropoffs": [
        {
          "entity_integration_key": "entity1",
          "shipping_address_integration_key": "shippingAddress1",
          "integration_key": "dropoff1"
          ...
        }
      ]

      ...
    }
  ]

  ...

```

## Adhoc Components

Some components such as Locations, Shipping Addresses and Entities have an `is_adhoc` property associated with them. When `is_adhoc` is set to true the component will not be created as master data but will instead only be appended to the route itself. Adhoc components are useful when there is no reliable business key for the component and saving them as master data will cause uncontrolled duplication. Where possible adhoc components should be avoided. In particular adhoc locations become very difficult to manage when the line of business system has unreliable geospatial information. The locations will need to be continuously managed from the Trackmatic front end making it impractical for operations to manage the locations, which will ultimately affect the quality of the data we produce.