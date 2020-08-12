#Webhooks Payloads
## Actions Dropoff Attempted `load.actiondropoff.attempted`
```
{
  "when": "2020-08-12T15:52:44.3394072Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "dropoffs": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "internal_reference": null,
      "due_at": "2020-08-12T15:52:44.3394072Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": null,
      "requirements": null
    }
  ],
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "started_at": "0001-01-01T00:00:00",
  "ended_at": "0001-01-01T00:00:00",
  "reason": "string",
  "comment": "string",
  "mobile": "string"
}
```
## Actions Dropoff Cancelled `load.actiondropoff.cancelled`
```
{
  "when": "2020-08-12T15:52:44.3404058Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "dropoffs": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "internal_reference": null,
      "due_at": "2020-08-12T15:52:44.3404058Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": null,
      "requirements": null
    }
  ],
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "started_at": "0001-01-01T00:00:00",
  "ended_at": "0001-01-01T00:00:00",
  "reason": "string",
  "comment": "string",
  "mobile": "string"
}
```
## Actions Dropoff Completed `load.actiondropoff.completed`
```
{
  "when": "2020-08-12T15:52:44.3374139Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "activity_id": null,
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "dropoffs": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "internal_reference": null,
      "due_at": "2020-08-12T15:52:44.3394072Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": null,
      "requirements": null
    }
  ],
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "resolutions": [
    {
      "dropoff_id": "string",
      "dropoff_reference": "string",
      "resolution_status": "string",
      "reason": "string",
      "comment": "string",
      "mobile_no": "string",
      "image_urls": [
        "string"
      ],
      "e_document_key": "string"
    }
  ],
  "started_at": "0001-01-01T00:00:00",
  "ended_at": "0001-01-01T00:00:00",
  "is_complete": false
}
```
## Actions Pickup Attempted `load.actionpickup.attempted`
```
{
  "when": "2020-08-12T15:52:44.341403Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "pickups": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "due_at": "2020-08-12T15:52:44.341403Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": null
    }
  ],
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "started_at": "0001-01-01T00:00:00",
  "ended_at": "0001-01-01T00:00:00",
  "reason": "string",
  "comment": "string",
  "mobile": "string"
}
```
## Actions Pickup Cancelled `load.actionpickup.cancelled`
```
{
  "when": "2020-08-12T15:52:44.341403Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "pickups": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "due_at": "2020-08-12T15:52:44.3424043Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": null
    }
  ],
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "started_at": "0001-01-01T00:00:00",
  "ended_at": "0001-01-01T00:00:00",
  "reason": "string",
  "comment": "string",
  "mobile": "string"
}
```
## Actions Pickup Completed `load.actionpickup.completed`
```
{
  "when": "2020-08-12T15:52:44.3404058Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "activity_id": null,
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "pickups": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "due_at": "2020-08-12T15:52:44.341403Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": null
    }
  ],
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "resolutions": [
    {
      "pickup_id": "string",
      "pickup_reference": "string",
      "resolution_status": "string",
      "reason": "string",
      "comment": "string",
      "mobile_no": "string",
      "image_urls": [
        "string"
      ],
      "e_document_key": "string"
    }
  ],
  "started_at": "0001-01-01T00:00:00",
  "ended_at": "0001-01-01T00:00:00",
  "is_complete": false
}
```
## Border Crossing `border_crossing`
```
{
  "when": "2020-08-12T15:52:44.3254514Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "country": "string",
  "name": "string",
  "money_order_number": "string",
  "border_permit_number": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  }
}
```
## Border Crossing Failed `border_crossing.failed`
```
{
  "when": "2020-08-12T15:52:44.3264417Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "failure_reason": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  }
}
```
## Breakdown `breakdown`
```
{
  "when": "2020-08-12T15:52:44.3334231Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "problematic_asset_id": null,
  "reason": null,
  "description": null,
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "driver_id": "string",
  "vehicle_id": "string",
  "problematic_asset_integration_key": null,
  "vehicle_integration_key": "string",
  "driver_integration_key": "string",
  "activity_id": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  }
}
```
## Collection Completed `collection.completed`
```
{
  "when": "2020-08-12T15:52:44.3443946Z",
  "where": [
    0.0
  ],
  "executed_activity_id": "string",
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "collection_attempted_outcome": {
    "reason": "string",
    "comment": "string",
    "mobile": "string",
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "collection_cancelled_outcome": {
    "reason": "string",
    "comment": "string",
    "mobile": "string",
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "collection_items_outcome": {
    "items": [
      {
        "handling_unit_id": "string",
        "barcode": "string",
        "description": "string",
        "quantity": 0,
        "barcode_captured": "string",
        "status": "string",
        "comment": "string",
        "reason": "string",
        "endorsement": {
          "reference": "string",
          "reason": "string",
          "comment": "string",
          "images": [
            "string"
          ]
        },
        "images": [
          "string"
        ]
      }
    ],
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "collection_parcels_defined_outcome": {
    "units": [
      {
        "handling_unit_id": "string",
        "barcode": null,
        "reference": null,
        "status": "string",
        "comment": "string",
        "reason": "string",
        "endorsement": {
          "reference": "string",
          "reason": "string",
          "comment": "string",
          "images": [
            "string"
          ]
        },
        "images": [
          "string"
        ]
      }
    ],
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "collection_parcels_undefined_outcome": {
    "units": [
      {
        "barcode": "string",
        "description": "string",
        "status": "string",
        "comment": "string",
        "reason": "string",
        "endorsement": {
          "reference": "string",
          "reason": "string",
          "comment": "string",
          "images": [
            "string"
          ]
        },
        "images": [
          "string"
        ]
      }
    ],
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "collection_parcels_unknown_outcome": {
    "waybill_no": "string",
    "quantity": 0,
    "images": [
      "string"
    ],
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  }
}
```
## Collection Started `load.collection.started`
```
{
  "when": "2020-08-12T15:52:44.343398Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "pickups": [
    {
      "id": "string",
      "integration_key": "string",
      "reference": "string",
      "due_at": "2020-08-12T15:52:44.343398Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": {
        "amount_incl": 0.0,
        "amount_excl": 0.0,
        "discount": 0.0
      },
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": [
        {
          "integration_key": "string",
          "first_name": "string",
          "last_name": "string",
          "mobile": "string",
          "work": "string",
          "email": "string"
        }
      ],
      "handling_units": [
        {
          "integrationkey": "string",
          "reference": "string",
          "description": "String",
          "customer_reference": "String",
          "internal_reference": "string",
          "barcode": "string",
          "dimensions": {
            "volumetric_mass": 0.0,
            "weight": 0.0,
            "pieces": 0,
            "pallets": 0.0,
            "volume": {
              "length": 0.0,
              "width": 0.0,
              "height": 0.0,
              "volume": 0.0
            },
            "litres": 0.0
          },
          "status": "string",
          "unit_of_measure": "string",
          "is_specified": false,
          "code": "string",
          "model": "String"
        }
      ]
    }
  ]
}
```
## Consignment Created `load.consignment.created`
```
{
  "when": "2020-08-12T15:52:44.3443946Z",
  "site_refrence": "string",
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": "string",
    "status": null,
    "pickups": [
      {
        "id": null,
        "integration_key": "string",
        "reference": null,
        "due_at": "2020-08-12T15:52:44.3453918Z",
        "quantity": {
          "value": 0.0,
          "units": "string"
        },
        "dimensions": {
          "volumetric_mass": 0.0,
          "weight": 0.0,
          "pieces": 0,
          "pallets": 0.0,
          "volume": {
            "length": 0.0,
            "width": 0.0,
            "height": 0.0,
            "volume": 0.0
          },
          "litres": 0.0
        },
        "financial": null,
        "maximum_service_time": "00:00:00",
        "entity": {
          "entity_id": "string",
          "name": "string",
          "integration_key": "string",
          "reference": null
        },
        "shipping_address": {
          "integration_key": "string",
          "name": null,
          "refernce": null,
          "shipping_address_id": "string",
          "unit_no": "string",
          "building_name": "string",
          "street_no": "string",
          "sub_division_number": "string",
          "street": "string",
          "suburb": "string",
          "city": "string",
          "province": "string",
          "postal_code": "string",
          "map_code": "string",
          "geofence": {
            "id": null,
            "integration_key": "string",
            "reference": "string",
            "name": "string",
            "entrance": [
              0.0,
              0.0
            ],
            "shape": {
              "markers": [
                [
                  0.0,
                  0.0
                ]
              ],
              "marker": [
                0.0,
                0.0
              ],
              "size": 0.0,
              "type": "string"
            }
          }
        },
        "contacts": null,
        "handling_units": [
          {
            "integrationkey": "string",
            "reference": "string",
            "description": "String",
            "customer_reference": "String",
            "internal_reference": "string",
            "barcode": "string",
            "dimensions": {
              "volumetric_mass": 0.0,
              "weight": 0.0,
              "pieces": 0,
              "pallets": 0.0,
              "volume": {
                "length": 0.0,
                "width": 0.0,
                "height": 0.0,
                "volume": 0.0
              },
              "litres": 0.0
            },
            "status": "string",
            "unit_of_measure": "string",
            "is_specified": false,
            "code": "string",
            "model": "String"
          }
        ]
      }
    ],
    "dropoffs": [
      {
        "id": null,
        "integration_key": "string",
        "reference": null,
        "internal_reference": null,
        "due_at": "2020-08-12T15:52:44.3453918Z",
        "quantity": {
          "value": 0.0,
          "units": "string"
        },
        "dimensions": {
          "volumetric_mass": 0.0,
          "weight": 0.0,
          "pieces": 0,
          "pallets": 0.0,
          "volume": {
            "length": 0.0,
            "width": 0.0,
            "height": 0.0,
            "volume": 0.0
          },
          "litres": 0.0
        },
        "financial": null,
        "maximum_service_time": "00:00:00",
        "entity": {
          "entity_id": "string",
          "name": "string",
          "integration_key": "string",
          "reference": null
        },
        "shipping_address": {
          "integration_key": "string",
          "name": null,
          "refernce": null,
          "shipping_address_id": "string",
          "unit_no": "string",
          "building_name": "string",
          "street_no": "string",
          "sub_division_number": "string",
          "street": "string",
          "suburb": "string",
          "city": "string",
          "province": "string",
          "postal_code": "string",
          "map_code": "string",
          "geofence": {
            "id": null,
            "integration_key": "string",
            "reference": "string",
            "name": "string",
            "entrance": [
              0.0,
              0.0
            ],
            "shape": {
              "markers": [
                [
                  0.0,
                  0.0
                ]
              ],
              "marker": [
                0.0,
                0.0
              ],
              "size": 0.0,
              "type": "string"
            }
          }
        },
        "contacts": null,
        "handling_units": [
          {
            "integrationkey": "string",
            "reference": "string",
            "description": "String",
            "customer_reference": "String",
            "internal_reference": "string",
            "barcode": "string",
            "dimensions": {
              "volumetric_mass": 0.0,
              "weight": 0.0,
              "pieces": 0,
              "pallets": 0.0,
              "volume": {
                "length": 0.0,
                "width": 0.0,
                "height": 0.0,
                "volume": 0.0
              },
              "litres": 0.0
            },
            "status": "string",
            "unit_of_measure": "string",
            "is_specified": null,
            "code": "string",
            "model": "String"
          }
        ],
        "requirements": null
      }
    ],
    "consignor": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "consignee": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "extension_property": [
      {
        "key": "string",
        "value": "string"
      }
    ]
  }
}
```
## Consignment Status Changed `load.consignment.status.changed`
```
{
  "when": "2020-08-12T15:52:44.3463896Z",
  "site_refrence": "string",
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": "string",
    "status": "string",
    "pickups": [
      {
        "id": null,
        "integration_key": "string",
        "reference": null,
        "due_at": "2020-08-12T15:52:44.3453918Z",
        "quantity": {
          "value": 0.0,
          "units": "string"
        },
        "dimensions": {
          "volumetric_mass": 0.0,
          "weight": 0.0,
          "pieces": 0,
          "pallets": 0.0,
          "volume": {
            "length": 0.0,
            "width": 0.0,
            "height": 0.0,
            "volume": 0.0
          },
          "litres": 0.0
        },
        "financial": null,
        "maximum_service_time": "00:00:00",
        "entity": {
          "entity_id": "string",
          "name": "string",
          "integration_key": "string",
          "reference": null
        },
        "shipping_address": {
          "integration_key": "string",
          "name": null,
          "refernce": null,
          "shipping_address_id": "string",
          "unit_no": "string",
          "building_name": "string",
          "street_no": "string",
          "sub_division_number": "string",
          "street": "string",
          "suburb": "string",
          "city": "string",
          "province": "string",
          "postal_code": "string",
          "map_code": "string",
          "geofence": {
            "id": null,
            "integration_key": "string",
            "reference": "string",
            "name": "string",
            "entrance": [
              0.0,
              0.0
            ],
            "shape": {
              "markers": [
                [
                  0.0,
                  0.0
                ]
              ],
              "marker": [
                0.0,
                0.0
              ],
              "size": 0.0,
              "type": "string"
            }
          }
        },
        "contacts": null,
        "handling_units": [
          {
            "integrationkey": "string",
            "reference": "string",
            "description": "String",
            "customer_reference": "String",
            "internal_reference": "string",
            "barcode": "string",
            "dimensions": {
              "volumetric_mass": 0.0,
              "weight": 0.0,
              "pieces": 0,
              "pallets": 0.0,
              "volume": {
                "length": 0.0,
                "width": 0.0,
                "height": 0.0,
                "volume": 0.0
              },
              "litres": 0.0
            },
            "status": "string",
            "unit_of_measure": "string",
            "is_specified": false,
            "code": "string",
            "model": "String"
          }
        ]
      }
    ],
    "dropoffs": [
      {
        "id": null,
        "integration_key": "string",
        "reference": null,
        "internal_reference": null,
        "due_at": "2020-08-12T15:52:44.3453918Z",
        "quantity": {
          "value": 0.0,
          "units": "string"
        },
        "dimensions": {
          "volumetric_mass": 0.0,
          "weight": 0.0,
          "pieces": 0,
          "pallets": 0.0,
          "volume": {
            "length": 0.0,
            "width": 0.0,
            "height": 0.0,
            "volume": 0.0
          },
          "litres": 0.0
        },
        "financial": null,
        "maximum_service_time": "00:00:00",
        "entity": {
          "entity_id": "string",
          "name": "string",
          "integration_key": "string",
          "reference": null
        },
        "shipping_address": {
          "integration_key": "string",
          "name": null,
          "refernce": null,
          "shipping_address_id": "string",
          "unit_no": "string",
          "building_name": "string",
          "street_no": "string",
          "sub_division_number": "string",
          "street": "string",
          "suburb": "string",
          "city": "string",
          "province": "string",
          "postal_code": "string",
          "map_code": "string",
          "geofence": {
            "id": null,
            "integration_key": "string",
            "reference": "string",
            "name": "string",
            "entrance": [
              0.0,
              0.0
            ],
            "shape": {
              "markers": [
                [
                  0.0,
                  0.0
                ]
              ],
              "marker": [
                0.0,
                0.0
              ],
              "size": 0.0,
              "type": "string"
            }
          }
        },
        "contacts": null,
        "handling_units": [
          {
            "integrationkey": "string",
            "reference": "string",
            "description": "String",
            "customer_reference": "String",
            "internal_reference": "string",
            "barcode": "string",
            "dimensions": {
              "volumetric_mass": 0.0,
              "weight": 0.0,
              "pieces": 0,
              "pallets": 0.0,
              "volume": {
                "length": 0.0,
                "width": 0.0,
                "height": 0.0,
                "volume": 0.0
              },
              "litres": 0.0
            },
            "status": "string",
            "unit_of_measure": "string",
            "is_specified": null,
            "code": "string",
            "model": "String"
          }
        ],
        "requirements": null
      }
    ],
    "consignor": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "consignee": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "extension_property": [
      {
        "key": "string",
        "value": "string"
      }
    ]
  }
}
```
## Custom Activity Completed `custom_activity.completed`
```
{
  "when": "2020-08-12T15:52:44.336415Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": null,
  "activity_id": "string",
  "activity_integration_key": "string"
}
```
## Custom Activity Started `custom_activity.started`
```
{
  "when": "2020-08-12T15:52:44.336415Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "activity_integration_key": "string",
  "activity_id": "string"
}
```
## Dropoff Completed `load.dropoff.completed`
```
{
  "when": "2020-08-12T15:52:44.3194617Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": null,
    "pickup_ids": null,
    "dropoff_ids": null,
    "consignor": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "consignee": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "status": null,
    "extension_property": null
  },
  "dropoff": {
    "id": null,
    "integration_key": "string",
    "reference": null,
    "internal_reference": null,
    "due_at": "2020-08-12T15:52:44.3204581Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
    },
    "dimensions": {
      "volumetric_mass": 0.0,
      "weight": 0.0,
      "pieces": 0,
      "pallets": 0.0,
      "volume": {
        "length": 0.0,
        "width": 0.0,
        "height": 0.0,
        "volume": 0.0
      },
      "litres": 0.0
    },
    "financial": null,
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string",
      "reference": null
    },
    "shipping_address": {
      "integration_key": "string",
      "name": null,
      "refernce": null,
      "shipping_address_id": "string",
      "unit_no": "string",
      "building_name": "string",
      "street_no": "string",
      "sub_division_number": "string",
      "street": "string",
      "suburb": "string",
      "city": "string",
      "province": "string",
      "postal_code": "string",
      "map_code": "string",
      "geofence": {
        "id": null,
        "integration_key": "string",
        "reference": "string",
        "name": "string",
        "entrance": [
          0.0,
          0.0
        ],
        "shape": {
          "markers": [
            [
              0.0,
              0.0
            ]
          ],
          "marker": [
            0.0,
            0.0
          ],
          "size": 0.0,
          "type": "string"
        }
      }
    },
    "contacts": null,
    "handling_units": [
      {
        "integrationkey": "string",
        "reference": "string",
        "description": "String",
        "customer_reference": "String",
        "internal_reference": "string",
        "barcode": "string",
        "dimensions": {
          "volumetric_mass": 0.0,
          "weight": 0.0,
          "pieces": 0,
          "pallets": 0.0,
          "volume": {
            "length": 0.0,
            "width": 0.0,
            "height": 0.0,
            "volume": 0.0
          },
          "litres": 0.0
        },
        "status": "string",
        "unit_of_measure": "string",
        "is_specified": false,
        "code": "string",
        "model": "String"
      }
    ],
    "requirements": null
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  }
}
```
## Dropoff Failed `load.dropoff.failed`
```
{
  "when": "2020-08-12T15:52:44.3244472Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": null,
    "pickup_ids": null,
    "dropoff_ids": null,
    "consignor": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "consignee": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "status": null,
    "extension_property": null
  },
  "dropoff": {
    "id": null,
    "integration_key": "string",
    "reference": null,
    "internal_reference": null,
    "due_at": "2020-08-12T15:52:44.3244472Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
    },
    "dimensions": {
      "volumetric_mass": 0.0,
      "weight": 0.0,
      "pieces": 0,
      "pallets": 0.0,
      "volume": {
        "length": 0.0,
        "width": 0.0,
        "height": 0.0,
        "volume": 0.0
      },
      "litres": 0.0
    },
    "financial": null,
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string",
      "reference": null
    },
    "shipping_address": {
      "integration_key": "string",
      "name": null,
      "refernce": null,
      "shipping_address_id": "string",
      "unit_no": "string",
      "building_name": "string",
      "street_no": "string",
      "sub_division_number": "string",
      "street": "string",
      "suburb": "string",
      "city": "string",
      "province": "string",
      "postal_code": "string",
      "map_code": "string",
      "geofence": {
        "id": null,
        "integration_key": "string",
        "reference": "string",
        "name": "string",
        "entrance": [
          0.0,
          0.0
        ],
        "shape": {
          "markers": [
            [
              0.0,
              0.0
            ]
          ],
          "marker": [
            0.0,
            0.0
          ],
          "size": 0.0,
          "type": "string"
        }
      }
    },
    "contacts": null,
    "handling_units": [
      {
        "integrationkey": "string",
        "reference": "string",
        "description": "String",
        "customer_reference": "String",
        "internal_reference": "string",
        "barcode": "string",
        "dimensions": {
          "volumetric_mass": 0.0,
          "weight": 0.0,
          "pieces": 0,
          "pallets": 0.0,
          "volume": {
            "length": 0.0,
            "width": 0.0,
            "height": 0.0,
            "volume": 0.0
          },
          "litres": 0.0
        },
        "status": "string",
        "unit_of_measure": "string",
        "is_specified": null,
        "code": "string",
        "model": "String"
      }
    ],
    "requirements": null
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "failure_reason": null
}
```
## Dropoff Started `load.dropoff.started`
```
{
  "when": "2020-08-12T15:52:44.3194617Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": null,
    "pickup_ids": null,
    "dropoff_ids": null,
    "consignor": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "consignee": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "status": null,
    "extension_property": null
  },
  "dropoff": {
    "id": null,
    "integration_key": "string",
    "reference": null,
    "internal_reference": null,
    "due_at": "2020-08-12T15:52:44.3194617Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
    },
    "dimensions": {
      "volumetric_mass": 0.0,
      "weight": 0.0,
      "pieces": 0,
      "pallets": 0.0,
      "volume": {
        "length": 0.0,
        "width": 0.0,
        "height": 0.0,
        "volume": 0.0
      },
      "litres": 0.0
    },
    "financial": null,
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string",
      "reference": null
    },
    "shipping_address": {
      "integration_key": "string",
      "name": null,
      "refernce": null,
      "shipping_address_id": "string",
      "unit_no": "string",
      "building_name": "string",
      "street_no": "string",
      "sub_division_number": "string",
      "street": "string",
      "suburb": "string",
      "city": "string",
      "province": "string",
      "postal_code": "string",
      "map_code": "string",
      "geofence": {
        "id": null,
        "integration_key": "string",
        "reference": "string",
        "name": "string",
        "entrance": [
          0.0,
          0.0
        ],
        "shape": {
          "markers": [
            [
              0.0,
              0.0
            ]
          ],
          "marker": [
            0.0,
            0.0
          ],
          "size": 0.0,
          "type": "string"
        }
      }
    },
    "contacts": null,
    "handling_units": null,
    "requirements": null
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  }
}
```
## Fuel Stop Completed `fuel_stop.completed`
```
{
  "when": "2020-08-12T15:52:44.3264417Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "authorized_location_geofence_id": null,
  "was_authorised_fuel_stop": false,
  "transactions": [
    {
      "location": null,
      "litres": 0.0,
      "cost": 0.0,
      "currency": "zar",
      "transaction_level": "full",
      "asset_id": "string",
      "asset_integration_key": "string",
      "odometer_reading": 0.0,
      "meter_type": null,
      "reference_number": null,
      "receipt_image_url": null
    }
  ],
  "activity_id": null,
  "driver_id": null,
  "vehicle_id": null,
  "was_planned": false,
  "vehicle_integration_key": null,
  "driver_integration_key": null,
  "activity_integration_key": null,
  "authorized_location_geofence_integration_key": null,
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  }
}
```
## Fuel Stop Failed `fuel_stop.failed`
```
{
  "when": "2020-08-12T15:52:44.3284359Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "failure_reason": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  }
}
```
## Fuel Stop Started `fuel_stop.started`
```
{
  "when": "2020-08-12T15:52:44.3264417Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "activity_id": null,
  "driver_id": null,
  "vehicle_id": null,
  "was_planned": false,
  "authorized_location_geofence_id": null,
  "vehicle_integration_key": null,
  "driver_integration_key": null,
  "activity_integration_key": null,
  "authorized_location_geofence_integration_key": null,
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  }
}
```
## Load Activated `load.activated`
```
{
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignments_summary": {
    "references": [
      "string"
    ],
    "total_volumetric_mass": 0.0,
    "total_weight": 0.0,
    "total_pieces": 0,
    "total_pallets": 0.0,
    "total_litres": 0.0,
    "total_volume": 0.0
  },
  "when": "2020-08-12T15:52:44.3154725Z",
  "where": [
    0.0,
    0.0
  ]
}
```
## Load Cancelled `load.cancelled`
```
{
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "when": "2020-08-12T15:52:44.3194617Z",
  "reason": "string"
}
```
## Load Claimed `load.claimed`
```
{
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "when": "2020-08-12T15:52:44.3344204Z",
  "where": [
    0.0,
    0.0
  ]
}
```
## Load Completed `load.completed`
```
{
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "travel_plan": null,
  "consignments": null,
  "pickups": null,
  "dropoffs": null,
  "execution": null,
  "force_closed": false,
  "when": "2020-08-12T15:52:44.3184647Z",
  "where": [
    0.0,
    0.0
  ]
}
```
## Load Expired `load.expired`
```
{
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "when": "2020-08-12T15:52:44.3184647Z"
}
```
## Load Planned `load.planned`
```
{
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "travel_plan": {
    "start": "2020-08-12T15:52:44.3184647Z",
    "end": "2020-08-12T15:52:44.3184647Z",
    "pois": [
      {
        "travel_plan_poi_id": "String",
        "due_time": "2020-08-12T15:52:44.3184647Z",
        "geofence_trackmatic_id": null,
        "geofence_id": "string",
        "geofence_name": "string",
        "tags": null,
        "activity_ids": null,
        "pickup_ids": null,
        "dropoff_ids": null,
        "activities": null
      }
    ]
  },
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "pickups": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "due_at": "2020-08-12T15:52:44.3174669Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": [
        {
          "integrationkey": "string",
          "reference": "string",
          "description": "String",
          "customer_reference": "String",
          "internal_reference": "string",
          "barcode": "string",
          "dimensions": {
            "volumetric_mass": 0.0,
            "weight": 0.0,
            "pieces": 0,
            "pallets": 0.0,
            "volume": {
              "length": 0.0,
              "width": 0.0,
              "height": 0.0,
              "volume": 0.0
            },
            "litres": 0.0
          },
          "status": "string",
          "unit_of_measure": "string",
          "is_specified": false,
          "code": "string",
          "model": "String"
        }
      ]
    }
  ],
  "dropoffs": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "internal_reference": null,
      "due_at": "2020-08-12T15:52:44.3164733Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": [
        {
          "integrationkey": "string",
          "reference": "string",
          "description": "String",
          "customer_reference": "String",
          "internal_reference": "string",
          "barcode": "string",
          "dimensions": {
            "volumetric_mass": 0.0,
            "weight": 0.0,
            "pieces": 0,
            "pallets": 0.0,
            "volume": {
              "length": 0.0,
              "width": 0.0,
              "height": 0.0,
              "volume": 0.0
            },
            "litres": 0.0
          },
          "status": "string",
          "unit_of_measure": "string",
          "is_specified": null,
          "code": "string",
          "model": "String"
        }
      ],
      "requirements": null
    }
  ],
  "when": "2020-08-12T15:52:44.3154725Z",
  "where": [
    0.0,
    0.0
  ]
}
```
## Load Released `load.released`
```
{
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "when": "2020-08-12T15:52:44.3344204Z",
  "where": [
    0.0,
    0.0
  ]
}
```
## Multi Dropoff Completed `load.multidropoff.completed`
```
{
  "when": "2020-08-12T15:52:44.3224527Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "activity_id": null,
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "dropoffs": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "internal_reference": null,
      "due_at": "2020-08-12T15:52:44.3224527Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": [
        {
          "integrationkey": "string",
          "reference": "string",
          "description": "String",
          "customer_reference": "String",
          "internal_reference": "string",
          "barcode": "string",
          "dimensions": {
            "volumetric_mass": 0.0,
            "weight": 0.0,
            "pieces": 0,
            "pallets": 0.0,
            "volume": {
              "length": 0.0,
              "width": 0.0,
              "height": 0.0,
              "volume": 0.0
            },
            "litres": 0.0
          },
          "status": "string",
          "unit_of_measure": "string",
          "is_specified": null,
          "code": "string",
          "model": "String"
        }
      ],
      "requirements": null
    }
  ],
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "resolutions": [
    {
      "dropoff_id": "string",
      "is_failure": false,
      "failure_reason": "string",
      "comment": "string",
      "returns": [
        {
          "qty": "0",
          "handling_unit_id": "string",
          "handling_unit_reference": null,
          "handling_unit_internal_reference": null,
          "handling_unit_customer_reference": null,
          "reference": "string",
          "reason": "string",
          "comment": "string"
        }
      ]
    }
  ],
  "unit_resolutions": [
    {
      "dropoff_id": "string",
      "dropoff_reference": "string",
      "unit_resolutions": [
        {
          "id": "string",
          "reference": "string",
          "barcode": "string",
          "internal_reference": "string",
          "customer_reference": "string",
          "status": "string",
          "comment": "string",
          "reason": "string",
          "endorsement": {
            "id": "string",
            "site_id": "string",
            "customer_reference": "string",
            "status": "string",
            "reason": "string",
            "comment": "string",
            "missing_sku_numbers": [
              {
                "barcode": "string",
                "quantity": 0
              }
            ],
            "excess_sku_numbers": [
              {
                "barcode": "string",
                "quantity": 0
              }
            ]
          },
          "images": [
            "string"
          ]
        }
      ],
      "signatures": [
        {
          "name": "string",
          "reference": "string",
          "comment": "string",
          "image_url": "string"
        }
      ],
      "is_failure": false,
      "failure_reason": "string",
      "comment": "string"
    }
  ],
  "started_at": "0001-01-01T00:00:00",
  "ended_at": "0001-01-01T00:00:00",
  "is_complete": false,
  "epods": null
}
```
## Multi Dropoff Failed `load.multidropoff.failed`
```
{
  "when": "2020-08-12T15:52:44.3224527Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "dropoffs": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "internal_reference": null,
      "due_at": "2020-08-12T15:52:44.3234495Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": [
        {
          "integrationkey": "string",
          "reference": "string",
          "description": "String",
          "customer_reference": "String",
          "internal_reference": "string",
          "barcode": "string",
          "dimensions": {
            "volumetric_mass": 0.0,
            "weight": 0.0,
            "pieces": 0,
            "pallets": 0.0,
            "volume": {
              "length": 0.0,
              "width": 0.0,
              "height": 0.0,
              "volume": 0.0
            },
            "litres": 0.0
          },
          "status": "string",
          "unit_of_measure": "string",
          "is_specified": null,
          "code": "string",
          "model": "String"
        }
      ],
      "requirements": null
    }
  ],
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "resolutions": [
    {
      "dropoff_id": "string",
      "is_failure": false,
      "failure_reason": "string",
      "comment": "string",
      "returns": [
        {
          "qty": "0",
          "handling_unit_id": "string",
          "handling_unit_reference": null,
          "handling_unit_internal_reference": null,
          "handling_unit_customer_reference": null,
          "reference": "string",
          "reason": "string",
          "comment": "string"
        }
      ]
    }
  ],
  "unit_resolutions": [
    {
      "dropoff_id": "string",
      "dropoff_reference": "string",
      "unit_resolutions": [
        {
          "id": "string",
          "reference": "string",
          "barcode": "string",
          "internal_reference": "string",
          "customer_reference": "string",
          "status": "string",
          "comment": "string",
          "reason": "string",
          "endorsement": {
            "id": "string",
            "site_id": "string",
            "customer_reference": "string",
            "status": "string",
            "reason": "string",
            "comment": "string",
            "missing_sku_numbers": [
              {
                "barcode": "string",
                "quantity": 0
              }
            ],
            "excess_sku_numbers": [
              {
                "barcode": "string",
                "quantity": 0
              }
            ]
          },
          "images": [
            "string"
          ]
        }
      ],
      "signatures": [
        {
          "name": "string",
          "reference": "string",
          "comment": "string",
          "image_url": "string"
        }
      ],
      "is_failure": false,
      "failure_reason": "string",
      "comment": "string"
    }
  ],
  "failure_reason": "string",
  "started_at": "0001-01-01T00:00:00",
  "ended_at": "0001-01-01T00:00:00",
  "is_complete": false
}
```
## Multi Dropoff Started `load.multidropoff.started`
```
{
  "when": "2020-08-12T15:52:44.3204581Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "dropoffs": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "internal_reference": null,
      "due_at": "2020-08-12T15:52:44.3214551Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": null,
      "requirements": null
    }
  ],
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  }
}
```
## Multi Pickup Completed `load.multipickup.completed`
```
{
  "when": "2020-08-12T15:52:44.3244472Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "activity_id": null,
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "pickups": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "due_at": "2020-08-12T15:52:44.3244472Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": [
        {
          "integrationkey": "string",
          "reference": "string",
          "description": "String",
          "customer_reference": "String",
          "internal_reference": "string",
          "barcode": "string",
          "dimensions": {
            "volumetric_mass": 0.0,
            "weight": 0.0,
            "pieces": 0,
            "pallets": 0.0,
            "volume": {
              "length": 0.0,
              "width": 0.0,
              "height": 0.0,
              "volume": 0.0
            },
            "litres": 0.0
          },
          "status": "string",
          "unit_of_measure": "string",
          "is_specified": false,
          "code": "string",
          "model": "String"
        }
      ]
    }
  ],
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "resolutions": [
    {
      "pickup_id": "string",
      "is_failure": false,
      "failure_reason": "string",
      "comment": "string"
    }
  ],
  "started_at": "0001-01-01T00:00:00",
  "ended_at": "0001-01-01T00:00:00",
  "is_complete": false
}
```
## Multi Pickup Failed `load.multipickup.failed`
```
{
  "when": "2020-08-12T15:52:44.3244472Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "pickups": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "due_at": "2020-08-12T15:52:44.3244472Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": [
        {
          "integrationkey": "string",
          "reference": "string",
          "description": "String",
          "customer_reference": "String",
          "internal_reference": "string",
          "barcode": "string",
          "dimensions": {
            "volumetric_mass": 0.0,
            "weight": 0.0,
            "pieces": 0,
            "pallets": 0.0,
            "volume": {
              "length": 0.0,
              "width": 0.0,
              "height": 0.0,
              "volume": 0.0
            },
            "litres": 0.0
          },
          "status": "string",
          "unit_of_measure": "string",
          "is_specified": false,
          "code": "string",
          "model": "String"
        }
      ]
    }
  ],
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "resolutions": [
    {
      "pickup_id": "string",
      "is_failure": false,
      "failure_reason": "string",
      "comment": "string"
    }
  ],
  "unit_resolutions": [
    {
      "dropoff_id": "string",
      "dropoff_reference": "string",
      "unit_resolutions": [
        {
          "id": "string",
          "reference": "string",
          "barcode": "string",
          "internal_reference": "string",
          "customer_reference": "string",
          "status": "string",
          "comment": "string",
          "reason": "string",
          "endorsement": {
            "id": "string",
            "site_id": "string",
            "customer_reference": "string",
            "status": "string",
            "reason": "string",
            "comment": "string",
            "missing_sku_numbers": [
              {
                "barcode": "string",
                "quantity": 0
              }
            ],
            "excess_sku_numbers": [
              {
                "barcode": "string",
                "quantity": 0
              }
            ]
          },
          "images": [
            "string"
          ]
        }
      ],
      "signatures": [
        {
          "name": "string",
          "reference": "string",
          "comment": "string",
          "image_url": "string"
        }
      ],
      "is_failure": false,
      "failure_reason": "string",
      "comment": "string"
    }
  ],
  "failure_reason": "string",
  "started_at": "0001-01-01T00:00:00",
  "ended_at": "0001-01-01T00:00:00",
  "is_complete": false
}
```
## Multi Pickup Started `load.multipickup.started`
```
{
  "when": "2020-08-12T15:52:44.3214551Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": null,
      "pickup_ids": null,
      "dropoff_ids": null,
      "consignor": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "consignee": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "status": null,
      "extension_property": null
    }
  ],
  "pickups": [
    {
      "id": null,
      "integration_key": "string",
      "reference": null,
      "due_at": "2020-08-12T15:52:44.3224527Z",
      "quantity": {
        "value": 0.0,
        "units": "string"
      },
      "dimensions": {
        "volumetric_mass": 0.0,
        "weight": 0.0,
        "pieces": 0,
        "pallets": 0.0,
        "volume": {
          "length": 0.0,
          "width": 0.0,
          "height": 0.0,
          "volume": 0.0
        },
        "litres": 0.0
      },
      "financial": null,
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
        "name": null,
        "refernce": null,
        "shipping_address_id": "string",
        "unit_no": "string",
        "building_name": "string",
        "street_no": "string",
        "sub_division_number": "string",
        "street": "string",
        "suburb": "string",
        "city": "string",
        "province": "string",
        "postal_code": "string",
        "map_code": "string",
        "geofence": {
          "id": null,
          "integration_key": "string",
          "reference": "string",
          "name": "string",
          "entrance": [
            0.0,
            0.0
          ],
          "shape": {
            "markers": [
              [
                0.0,
                0.0
              ]
            ],
            "marker": [
              0.0,
              0.0
            ],
            "size": 0.0,
            "type": "string"
          }
        }
      },
      "contacts": null,
      "handling_units": null
    }
  ],
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  }
}
```
## Odometer `odometer`
```
{
  "id": null,
  "activity_id": null,
  "when": "2020-08-12T15:52:44.3294329Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "asset_id": "string",
  "asset_integration_key": null,
  "meter_reading": 0.0,
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "was_planned": false,
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  }
}
```
## Odometer Failed `odometer.failed`
```
{
  "when": "2020-08-12T15:52:44.3304303Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "failure_reason": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  }
}
```
## Off Route `off_route`
```
{
  "when": "2020-08-12T15:52:44.3334231Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  }
}
```
## Pickup Completed `load.pickup.completed`
```
{
  "when": "2020-08-12T15:52:44.3254514Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": null,
    "pickup_ids": null,
    "dropoff_ids": null,
    "consignor": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "consignee": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "status": null,
    "extension_property": null
  },
  "pickup": {
    "id": null,
    "integration_key": "string",
    "reference": null,
    "due_at": "2020-08-12T15:52:44.3254514Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
    },
    "dimensions": {
      "volumetric_mass": 0.0,
      "weight": 0.0,
      "pieces": 0,
      "pallets": 0.0,
      "volume": {
        "length": 0.0,
        "width": 0.0,
        "height": 0.0,
        "volume": 0.0
      },
      "litres": 0.0
    },
    "financial": null,
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string",
      "reference": null
    },
    "shipping_address": {
      "integration_key": "string",
      "name": null,
      "refernce": null,
      "shipping_address_id": "string",
      "unit_no": "string",
      "building_name": "string",
      "street_no": "string",
      "sub_division_number": "string",
      "street": "string",
      "suburb": "string",
      "city": "string",
      "province": "string",
      "postal_code": "string",
      "map_code": "string",
      "geofence": {
        "id": null,
        "integration_key": "string",
        "reference": "string",
        "name": "string",
        "entrance": [
          0.0,
          0.0
        ],
        "shape": {
          "markers": [
            [
              0.0,
              0.0
            ]
          ],
          "marker": [
            0.0,
            0.0
          ],
          "size": 0.0,
          "type": "string"
        }
      }
    },
    "contacts": null,
    "handling_units": [
      {
        "integrationkey": "string",
        "reference": "string",
        "description": "String",
        "customer_reference": "String",
        "internal_reference": "string",
        "barcode": "string",
        "dimensions": {
          "volumetric_mass": 0.0,
          "weight": 0.0,
          "pieces": 0,
          "pallets": 0.0,
          "volume": {
            "length": 0.0,
            "width": 0.0,
            "height": 0.0,
            "volume": 0.0
          },
          "litres": 0.0
        },
        "status": "string",
        "unit_of_measure": "string",
        "is_specified": false,
        "code": "string",
        "model": "String"
      }
    ]
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  }
}
```
## Pickup Failed `load.pickup.failed`
```
{
  "when": "2020-08-12T15:52:44.3254514Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": null,
    "pickup_ids": null,
    "dropoff_ids": null,
    "consignor": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "consignee": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "status": null,
    "extension_property": null
  },
  "pickup": {
    "id": null,
    "integration_key": "string",
    "reference": null,
    "due_at": "2020-08-12T15:52:44.3254514Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
    },
    "dimensions": {
      "volumetric_mass": 0.0,
      "weight": 0.0,
      "pieces": 0,
      "pallets": 0.0,
      "volume": {
        "length": 0.0,
        "width": 0.0,
        "height": 0.0,
        "volume": 0.0
      },
      "litres": 0.0
    },
    "financial": null,
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string",
      "reference": null
    },
    "shipping_address": {
      "integration_key": "string",
      "name": null,
      "refernce": null,
      "shipping_address_id": "string",
      "unit_no": "string",
      "building_name": "string",
      "street_no": "string",
      "sub_division_number": "string",
      "street": "string",
      "suburb": "string",
      "city": "string",
      "province": "string",
      "postal_code": "string",
      "map_code": "string",
      "geofence": {
        "id": null,
        "integration_key": "string",
        "reference": "string",
        "name": "string",
        "entrance": [
          0.0,
          0.0
        ],
        "shape": {
          "markers": [
            [
              0.0,
              0.0
            ]
          ],
          "marker": [
            0.0,
            0.0
          ],
          "size": 0.0,
          "type": "string"
        }
      }
    },
    "contacts": null,
    "handling_units": [
      {
        "integrationkey": "string",
        "reference": "string",
        "description": "String",
        "customer_reference": "String",
        "internal_reference": "string",
        "barcode": "string",
        "dimensions": {
          "volumetric_mass": 0.0,
          "weight": 0.0,
          "pieces": 0,
          "pallets": 0.0,
          "volume": {
            "length": 0.0,
            "width": 0.0,
            "height": 0.0,
            "volume": 0.0
          },
          "litres": 0.0
        },
        "status": "string",
        "unit_of_measure": "string",
        "is_specified": false,
        "code": "string",
        "model": "String"
      }
    ]
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "failure_reason": null
}
```
## Pickup Started `load.pickup.started`
```
{
  "when": "2020-08-12T15:52:44.3244472Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": null,
    "pickup_ids": null,
    "dropoff_ids": null,
    "consignor": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "consignee": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string"
    },
    "status": null,
    "extension_property": null
  },
  "pickup": {
    "id": null,
    "integration_key": "string",
    "reference": null,
    "due_at": "2020-08-12T15:52:44.3254514Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
    },
    "dimensions": {
      "volumetric_mass": 0.0,
      "weight": 0.0,
      "pieces": 0,
      "pallets": 0.0,
      "volume": {
        "length": 0.0,
        "width": 0.0,
        "height": 0.0,
        "volume": 0.0
      },
      "litres": 0.0
    },
    "financial": null,
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string",
      "reference": null
    },
    "shipping_address": {
      "integration_key": "string",
      "name": null,
      "refernce": null,
      "shipping_address_id": "string",
      "unit_no": "string",
      "building_name": "string",
      "street_no": "string",
      "sub_division_number": "string",
      "street": "string",
      "suburb": "string",
      "city": "string",
      "province": "string",
      "postal_code": "string",
      "map_code": "string",
      "geofence": {
        "id": null,
        "integration_key": "string",
        "reference": "string",
        "name": "string",
        "entrance": [
          0.0,
          0.0
        ],
        "shape": {
          "markers": [
            [
              0.0,
              0.0
            ]
          ],
          "marker": [
            0.0,
            0.0
          ],
          "size": 0.0,
          "type": "string"
        }
      }
    },
    "contacts": null,
    "handling_units": null
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  }
}
```
## Process Edocs Response `edoc.process.response`
```
{
  "when": "2020-08-12T15:52:44.3424043Z",
  "where": [
    0.0,
    0.0
  ],
  "document_url": "string",
  "document": "string",
  "document_key": "string",
  "document_type": "string",
  "load_id": "string",
  "consignment_reference": "string",
  "success": false,
  "error_message": "string"
}
```
## Rest Stop Completed `rest_stop.completed`
```
{
  "when": "2020-08-12T15:52:44.3284359Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "planned_duration": "00:00:00",
  "comments": "string",
  "reason": "string",
  "outcomes": {
    "signatures": [],
    "cash_on_deliveries": [],
    "document_scans": [],
    "images": [],
    "service_ratings": [],
    "odometer_readings": [],
    "pallet_transfers": [],
    "proof_of_deliveries": [],
    "weights": [],
    "forms": [],
    "e_documents": [],
    "delays": [],
    "contactless_confirmations": []
  },
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  },
  "reference_number": null
}
```
## Rest Stop Failed `rest_stop.failed`
```
{
  "when": "2020-08-12T15:52:44.3294329Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "failure_reason": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  },
  "reference_number": null
}
```
## Rest Stop Started `rest_stop.started`
```
{
  "when": "2020-08-12T15:52:44.3284359Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "planned_duration": "00:00:00",
  "comments": "string",
  "reason": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  },
  "reference_number": "string"
}
```
## Stop Arrived `load.stop.arrived`
```
{
  "when": "2020-08-12T15:52:44.314476Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "travel_plan_poi_id": "string",
  "activity_ids": null,
  "shipping_addresses": null,
  "integration_key": "string"
}
```
## Stop Departed `load.stop.departed`
```
{
  "when": "2020-08-12T15:52:44.3154725Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "travel_plan_poi_id": "string",
  "activity_ids": null,
  "shipping_addresses": null,
  "integration_key": "string"
}
```
## Stop Failed `load.stop.failed`
```
{
  "when": "2020-08-12T15:52:44.3304303Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "failure_reason": "string"
}
```
## Stop Recorded `load.stop.recorded`
```
{
  "when": "2020-08-12T15:52:44.3304303Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "travel_plan_poi_id": null,
  "integration_key": null
}
```
## Timed Task Completed `timed_task.completed`
```
{
  "when": "2020-08-12T15:52:44.335418Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": null,
  "activity_id": "string",
  "activity_integration_key": "string"
}
```
## Timed Task Failed `timed_task.failed`
```
{
  "when": "2020-08-12T15:52:44.335418Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": null,
  "failure_reason": null,
  "activity_id": "string",
  "activity_integration_key": "string"
}
```
## Timed Task Started `timed_task.started`
```
{
  "when": "2020-08-12T15:52:44.3344204Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "activity_integration_key": "string",
  "activity_id": "string"
}
```
## Travel Plan Updated `load.travelplan.updated`
```
{
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "travel_plan": {
    "start": "2020-08-12T15:52:44.3453918Z",
    "end": "2020-08-12T15:52:44.3453918Z",
    "pois": [
      {
        "travel_plan_poi_id": "string",
        "due_time": "2020-08-12T15:52:44.3453918Z",
        "geofence_trackmatic_id": null,
        "geofence_id": "string",
        "geofence_name": "string",
        "tags": [],
        "activity_ids": [],
        "pickup_ids": [],
        "dropoff_ids": [],
        "activities": null
      }
    ]
  },
  "when": "2020-08-12T15:52:44.3453918Z"
}
```
## Weighbridge Completed `weighbridge.completed`
```
{
  "when": "2020-08-12T15:52:44.3314279Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "was_planned": false,
  "weighbridge_name": "string",
  "failed": false,
  "reason_for_failure": "string",
  "failure_description": "string",
  "total_mass": 0.0,
  "overloaded_by": 0.0,
  "fine_reference_no": "string",
  "fine_amount": 0.0,
  "fine_amount_currency": "string",
  "activity_id": "string",
  "driver_id": "string",
  "vehicle_id": "string",
  "vehicle_integration_key": "string",
  "driver_integration_key": "string",
  "activity_integration_key": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  }
}
```
## Weighbridge Failed `weighbridge.failed`
```
{
  "when": "2020-08-12T15:52:44.3324261Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "cash_on_deliveries": [
      {
        "stock_handed_over": false,
        "reference": "string",
        "payment_received_by": 0,
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "document_scans": [
      {
        "image_urls": [
          "string"
        ],
        "comment": "string",
        "type": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "images": [
      {
        "image_urls": [
          "string"
        ],
        "comments": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_id": "string",
        "asset_integration_key": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "integration_key": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "e_documents": [
      {
        "documents": [
          {
            "key": "String",
            "document_type": "String",
            "document_name": "String",
            "signee_name": "String",
            "comment": "String",
            "completed_on": "2020-08-12T15:52:44.3114816Z"
          }
        ],
        "outcome_type": null,
        "integration_key": "String",
        "status": "String",
        "status_reason": "String"
      }
    ],
    "delays": [
      {
        "is_delayed": false,
        "reason": "string",
        "comment": "string",
        "outcome_type": null,
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "contactless_confirmations": []
  },
  "failure_reason": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  }
}
```
## Weighbridge Started `weighbridge.started`
```
{
  "when": "2020-08-12T15:52:44.3304303Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "organisation_id": null,
    "site_id": "string",
    "site_name": null,
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "name": null,
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "identity_number_prefix": null,
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "identity_number_prefix": null,
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0,
        "tags": null
      },
      "assets": [
        {
          "integration_key": "string",
          "asset_id": "string",
          "fleet_number": "string",
          "odometer": {
            "meter_type": "string",
            "current_reading": 0.0
          },
          "type": "string",
          "tags": null
        }
      ],
      "accessories": {
        "pallet_jack": "string",
        "load_lock_rails": 0,
        "fuel_card": "string"
      }
    },
    "type": "string",
    "created_by": "string"
  },
  "activity_id": "string",
  "driver_id": "string",
  "vehicle_id": "string",
  "was_planned": false,
  "weighbridge_name": "string",
  "vehicle_integration_key": "string",
  "driver_integration_key": "string",
  "activity_integration_key": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "identity_number_prefix": null,
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0,
    "tags": null
  }
}
```