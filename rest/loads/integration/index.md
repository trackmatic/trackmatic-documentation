# Integration Api

The integration API provides a way to upload the complex load structure in a normalized format. There are many moving parts to a load and care should be taken when building an integration to ensure a reliable and robust result.

Each message represents a single load along with all of its associated data. Once initial validation has been performed on the message the load is dispatched asynchrnously to be processed by the server. This means that the load may not be available immediately after a 200 response code is received. A web hook can be registered to notify you once the upload is complete.

## Open Api Documentation
For more information on available calls and messages structure [goto the open api docs](./open-api)

## Validation

The message you construct and send goes through a series of validation steps. The first phase does basic type checking and ensures that required fields have been provide. The next phase checks the referential integrity of the message. Lookup data is scanned for duplicates and lookup references are checked for consistency. If any failures are detected the API will respond with a "400 Bad Request" http status code. Details of the failure will be contained in the response message.

## Data Ownership

The data ownership component of the message is an important mechanism providing control over the ownership of various elements of the message. Using the data ownership component you are able to configure the behavior of the API for create, update and delete operations of the supported areas. The options for the operations are as follows:

- Accept - This will instruct the API to accept changes sent within the message and overwrite any data which already exists in the Trackmatic system. Using this option makes your system the owner of the data area.

- Throw Error - This option will instruct the api to throw an error if the operation is attempted. This is useful when debugging or if you are not certain of the effect that the message will have on the data.

- Ignore - When using this option the api will ignore any data sent by you if the data already exists in Trackmatic. This effectively makes Trackmatic the owner of the data area since once a component is created any further changes made by this api call will be ignored. This is usefull for when you need to allow chanegs to me made through the Trackmatic user interface and not have them overwritten by the integration.

## Integration Keys

The integration key properties are intended to represent either your business keys or composite business keys which you created. This is useful for performing updates since you will not be required to call our API to get the trackmatic id, instead you simply send the message again. If the integration keys macthes data which has been previously uploaded an update will be performed. If an integration does not exist in the trackmatic system a create will be performed.

Intgeration keys are mapped to trackmatic id's internally. When working with non integration apis or the Trackamtic web interface you will be working with trackmatic id's.

When webhooks are created the integration keys are retrieved and populated into the webhook payload so that you can correlate the webhook data with your line of business systems.

### Normalization

The payload allows you to upload supporting data in a normalized fashion. Each component can be defined once then referenced in other parts of the message using their integration keys.

```

  "geofences": [
    {
      "integration_key": "geofence1"
    }
  ],

  "shipping_addresses": [
    {
      "integration_key": "shippingAddress1",
      "geofence_integration_key": "geofence1"

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

## Consignments

Consignments represent the goods being moved and allow you to defined one or more pickup and dropoff activities for those goods.

The sequence and timing of the pickups and dropoffs are configured in the load travel plan.

## Entities

Entities define the busines entity which can play multiple roles within a load. An entity can either be a consignor, consignee or pickup/dropoff entity.

## Shipping Addresses

Shipping addresses represent the pickup or dropoff address information for the relevant entities. A shipping address is different to a geofence in that it describes the business address where the geofence describes the physical location which th driver will be visiting.

## Geofence

The geofences describes the physical location on the planet which the driver must visit. It requires an entrance and a shape field to be valid. The entrance describe the lon/lat of where the vehicle will enter the geofence, while the shape allows you to draw a boundary around the physical location. The system uses this boundary to determine when the vehicle arrives at or leaves a point of intetrest. The shape can either be defined as a radius or polygon.

## Planned Activities

Planned activities allow you to instruct the driver to perform specifc activities at a given point of interest. The sequence of the planned activities are configured in the load travel plan. 

## Activation & Completion

The actication and completion elements allow you to define requirements which need to be fullfilled when a driver activates or completes a load.

This feature is useful when you require a driver to capture information which is related to any specific point of interest.

## Load

The load is made up of one or more consignments which need to be fulfilled, the allocation of a driver, crew and assets as well as the travel plan.

### Travel Plan

The travel plan describes the sequence of events that the driver should follow in order to execute a load. A plan is made up of 2 or more points of interest. The the driver arrives at a point of interest he will be requested to execute the defined activities.

It is up to you to provide the sequence of the travel plan. You can let the system calculate the travel path between the points of interest or you an provide that information yourself from your own planning tools.

### Activities

Activities describe work to be performed by the driver at a point of interest. There are multiple types of activities namely:

- Pickups
- Dropoffs
- Odometer readings
- Rest stops
- Fatigue assessments
- Border crossings
- Weighbridges
- Fuel stops
- Pallet drops

Each activity has zero or more requirements which describes a workflow the the driver must follow in order to complete the activity.

The requirements are intended to allow you to customise the workflow of a visit. Each requirement is a building block which you can use to create more complex workflows. The supported requirements are as follows:

- Signatures
- Cash on delivery
- Document scans
- Image cpature
- Odometer readings
- Pallet transfers
- Pallet drops
- Service ratings
- Proof of deliveries
- Weighbridge readings
- E-Documents

Each activity can describe a success and failure requirment workflow.