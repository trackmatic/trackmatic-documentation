******
Import
******

The import API provides a way to upload the complex load structure in a denormalized format. There are many moving parts to a load and care should be taken when building an integration to ensure a reliable and robust result.

Each message represents a single load along with all of its associated data. Once initial validation has been performed on the message the load is dispatched asynchrnously to be processed by the server. This means that the load may not be available immediately after a 200 response code is received. A web hook can be registered to notify you once the upload is complete.

Validation
==========

The message you construct and send goes through a series of validation steps. The first phase does basic type checking and ensures that required fields have been provide. The next phase checks the referential integrity of the message. Lookup data is scanned for duplicates and lookup references are checked for consistency. If any failures are detected the API will respond with a "400 Bad Request" http status code. Details of the failure will be contained in the response message.

Validation
==========

The data ownership component of the message is an important mechanism providing control over the ownership of various elements of the message. Using the data ownership component you are able to configure the behavior of the API for create, update and delete operations of the supported areas. The options for the operations are as follows:

- Accept - This will instruct the API to accept changes sent within the message and overwrite any data which already exists in the Trackmatic system. Using this option makes your system the owner of the data area.

- Throw Error - This option will instruct the api to throw an error if the operation is attempted. This is useful when debugging or if you are not certain of the effect that the message will have on the data.

- Ignore - When using this option the api will ignore any data sent by you if the data already exists in Trackmatic. This effectively makes Trackmatic the owner of the data area since once a component is created any further changes made by this api call will be ignored. This is usefull for when you need to allow chanegs to me made through the Trackmatic user interface and not have them overwritten by the integration.

References
==========

The various components are linked together by their respective references within the payload. The reference fields are intended to be populated with your business keys for the various elements of the payload. The reference number will follow the data through into the webhooks which will allow you to correlate the data in the webhook messages. The pattern is used throughout the message structure. 

This process helps with deduplicating data within the payload. For example, when uploading a consignment with an associated entity, shipping address and geofence the payload would appear as follows:

.. code-block::

  "geofences": [
    {
      "reference": "geofence1"
    }
  ],

  "shipping_addresses": [
    {
      "reference": "shippingAddress1",
      "geofence_reference": "geofence1"

      ...
    }
  ],
  "entities": [
    {
      "reference": "entity1"

      ...
    }
  ],
  "consignments": [
    {
      "reference": "consignment1",
      "dropoffs": [
        {
          "entity_reference": "entity1",
          "shipping_address_reference": "shippingAddress1",
          "reference": "dropoff1"
          ...
        }
      ]

      ...
    }
  ]

  ...
