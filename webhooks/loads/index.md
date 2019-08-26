#Webhooks Payloads
## Actions Dropoff Attempted `load.actiondropoff.attempted`
```
{
  "when": "2019-08-26T06:57:47.5539411Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "internal_reference": null,
      "due_at": "2019-08-26T06:57:47.5549404Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
  "when": "2019-08-26T06:57:47.5549404Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "internal_reference": null,
      "due_at": "2019-08-26T06:57:47.5549404Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
  "when": "2019-08-26T06:57:47.5539411Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "internal_reference": null,
      "due_at": "2019-08-26T06:57:47.5539411Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
  "when": "2019-08-26T06:57:47.555975Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
      }
    }
  ],
  "pickups": [
    {
      "integration_key": "string",
      "due_at": "2019-08-26T06:57:47.5569371Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
  "when": "2019-08-26T06:57:47.5569371Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
      }
    }
  ],
  "pickups": [
    {
      "integration_key": "string",
      "due_at": "2019-08-26T06:57:47.5569371Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
  "when": "2019-08-26T06:57:47.555975Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
      }
    }
  ],
  "pickups": [
    {
      "integration_key": "string",
      "due_at": "2019-08-26T06:57:47.555975Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
  "when": "2019-08-26T06:57:47.5389361Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "country": "string",
  "name": "string",
  "money_order_number": "string",
  "border_permit_number": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  }
}
```
## Border Crossing Failed `border_crossing.failed`
```
{
  "when": "2019-08-26T06:57:47.5389361Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "failure_reason": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  }
}
```
## Breakdown `breakdown`
```
{
  "when": "2019-08-26T06:57:47.5489716Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  }
}
```
## Collection Completed `collection.completed`
```
{
  "when": "2019-08-26T06:57:47.5589368Z",
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
      }
    }
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  }
}
```
## Custom Activity Completed `custom_activity.completed`
```
{
  "when": "2019-08-26T06:57:47.5519395Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "when": "2019-08-26T06:57:47.5519395Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "when": "2019-08-26T06:57:47.5339315Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
    }
  },
  "dropoff": {
    "integration_key": "string",
    "internal_reference": null,
    "due_at": "2019-08-26T06:57:47.5339315Z",
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
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string",
      "reference": null
    },
    "shipping_address": {
      "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  }
}
```
## Dropoff Failed `load.dropoff.failed`
```
{
  "when": "2019-08-26T06:57:47.5369362Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
    }
  },
  "dropoff": {
    "integration_key": "string",
    "internal_reference": null,
    "due_at": "2019-08-26T06:57:47.5379361Z",
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
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string",
      "reference": null
    },
    "shipping_address": {
      "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "failure_reason": null
}
```
## Dropoff Started `load.dropoff.started`
```
{
  "when": "2019-08-26T06:57:47.5339315Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
    }
  },
  "dropoff": {
    "integration_key": "string",
    "internal_reference": null,
    "due_at": "2019-08-26T06:57:47.5339315Z",
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
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string",
      "reference": null
    },
    "shipping_address": {
      "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  }
}
```
## Fuel Stop Completed `fuel_stop.completed`
```
{
  "when": "2019-08-26T06:57:47.5409333Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  }
}
```
## Fuel Stop Failed `fuel_stop.failed`
```
{
  "when": "2019-08-26T06:57:47.5419395Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "failure_reason": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  }
}
```
## Fuel Stop Started `fuel_stop.started`
```
{
  "when": "2019-08-26T06:57:47.5399359Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  }
}
```
## Load Activated `load.activated`
```
{
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "when": "2019-08-26T06:57:47.5299672Z",
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
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "when": "2019-08-26T06:57:47.5329322Z",
  "reason": "string"
}
```
## Load Claimed `load.claimed`
```
{
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "when": "2019-08-26T06:57:47.5499328Z",
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
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "force_closed": false,
  "when": "2019-08-26T06:57:47.5329322Z",
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
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "when": "2019-08-26T06:57:47.5329322Z"
}
```
## Load Planned `load.planned`
```
{
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
    "start": "2019-08-26T06:57:47.5319367Z",
    "end": "2019-08-26T06:57:47.5319367Z",
    "pois": [
      {
        "travel_plan_poi_id": "String",
        "due_time": "2019-08-26T06:57:47.5329322Z",
        "geofence_id": "string",
        "geofence_name": "string",
        "activity_ids": null
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
      }
    }
  ],
  "pickups": [
    {
      "integration_key": "string",
      "due_at": "2019-08-26T06:57:47.5319367Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
      "integration_key": "string",
      "internal_reference": null,
      "due_at": "2019-08-26T06:57:47.5309366Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
  "when": "2019-08-26T06:57:47.5299672Z",
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
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "when": "2019-08-26T06:57:47.5499328Z",
  "where": [
    0.0,
    0.0
  ]
}
```
## Multi Dropoff Completed `load.multidropoff.completed`
```
{
  "when": "2019-08-26T06:57:47.534936Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "internal_reference": null,
      "due_at": "2019-08-26T06:57:47.5359364Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
  "when": "2019-08-26T06:57:47.5359364Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "internal_reference": null,
      "due_at": "2019-08-26T06:57:47.5359364Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
  "when": "2019-08-26T06:57:47.5339315Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "internal_reference": null,
      "due_at": "2019-08-26T06:57:47.534936Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  }
}
```
## Multi Pickup Completed `load.multipickup.completed`
```
{
  "when": "2019-08-26T06:57:47.5359364Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
      }
    }
  ],
  "pickups": [
    {
      "integration_key": "string",
      "due_at": "2019-08-26T06:57:47.5369362Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
## Multi Pickup Failed `load.multidropoff.failed`
```
{
  "when": "2019-08-26T06:57:47.5359364Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "internal_reference": null,
      "due_at": "2019-08-26T06:57:47.5359364Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
  "when": "2019-08-26T06:57:47.534936Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
      }
    }
  ],
  "pickups": [
    {
      "integration_key": "string",
      "due_at": "2019-08-26T06:57:47.534936Z",
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
      "maximum_service_time": "00:00:00",
      "entity": {
        "entity_id": "string",
        "name": "string",
        "integration_key": "string",
        "reference": null
      },
      "shipping_address": {
        "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  }
}
```
## Odometer `odometer`
```
{
  "id": null,
  "when": "2019-08-26T06:57:47.5439346Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "was_planned": false,
  "driver": {
    "id": "string",
    "name": "string",
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  }
}
```
## Odometer Failed `odometer.failed`
```
{
  "when": "2019-08-26T06:57:47.5449372Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "failure_reason": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  }
}
```
## Off Route `off_route`
```
{
  "when": "2019-08-26T06:57:47.5489716Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "when": "2019-08-26T06:57:47.5379361Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
    }
  },
  "pickup": {
    "integration_key": "string",
    "due_at": "2019-08-26T06:57:47.5379361Z",
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
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string",
      "reference": null
    },
    "shipping_address": {
      "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  }
}
```
## Pickup Failed `load.pickup.failed`
```
{
  "when": "2019-08-26T06:57:47.5379361Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
    }
  },
  "pickup": {
    "integration_key": "string",
    "due_at": "2019-08-26T06:57:47.5389361Z",
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
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string",
      "reference": null
    },
    "shipping_address": {
      "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "failure_reason": null
}
```
## Pickup Started `load.pickup.started`
```
{
  "when": "2019-08-26T06:57:47.5379361Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
    }
  },
  "pickup": {
    "integration_key": "string",
    "due_at": "2019-08-26T06:57:47.5379361Z",
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
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "integration_key": "string",
      "reference": null
    },
    "shipping_address": {
      "integration_key": "string",
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  }
}
```
## Process Edocs Response `edoc.process.response`
```
{
  "when": "2019-08-26T06:57:47.5579369Z",
  "where": [
    0.0,
    0.0
  ],
  "document_url": "string",
  "document_key": "string",
  "load_id": "string",
  "success": false,
  "error_message": "string"
}
```
## Rest Stop Completed `rest_stop.completed`
```
{
  "when": "2019-08-26T06:57:47.5429343Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
    "delays": []
  },
  "driver": {
    "id": "string",
    "name": "string",
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  },
  "reference_number": null
}
```
## Rest Stop Failed `rest_stop.failed`
```
{
  "when": "2019-08-26T06:57:47.5439346Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "failure_reason": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  },
  "reference_number": null
}
```
## Rest Stop Started `rest_stop.started`
```
{
  "when": "2019-08-26T06:57:47.5429343Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  },
  "reference_number": "string"
}
```
## Stop Arrived `load.stop.arrived`
```
{
  "when": "2019-08-26T06:57:47.5279365Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "integration_key": "string"
}
```
## Stop Departed `load.stop.departed`
```
{
  "when": "2019-08-26T06:57:47.5289408Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "integration_key": "string"
}
```
## Stop Failed `load.stop.failed`
```
{
  "when": "2019-08-26T06:57:47.5459372Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "failure_reason": "string"
}
```
## Stop Recorded `load.stop.recorded`
```
{
  "when": "2019-08-26T06:57:47.5459372Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "travel_plan_poi_id": null,
  "integration_key": null
}
```
## Timed Task Completed `timed_task.completed`
```
{
  "when": "2019-08-26T06:57:47.5509322Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "when": "2019-08-26T06:57:47.5519395Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
  "when": "2019-08-26T06:57:47.5499328Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
## Weighbridge Completed `weighbridge.completed`
```
{
  "when": "2019-08-26T06:57:47.5469325Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
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
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  }
}
```
## Weighbridge Failed `weighbridge.failed`
```
{
  "when": "2019-08-26T06:57:47.5489716Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
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
            "completed_on": "2019-08-26T06:57:47.5239339Z"
          }
        ],
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
        "integration_key": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "failure_reason": "string",
  "driver": {
    "id": "string",
    "name": "string",
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  }
}
```
## Weighbridge Started `weighbridge.started`
```
{
  "when": "2019-08-26T06:57:47.5459372Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": "string",
    "site_id": "string",
    "integration_key": "string",
    "requested_date": "0001-01-01T00:00:00",
    "date_created": "0001-01-01T00:00:00",
    "reference": "string",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "integration_key": "string"
      },
      "crew": [
        {
          "id": "string",
          "name": "string",
          "integration_key": "string"
        }
      ],
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string",
        "odometer": 0.0
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
          "type": "string"
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
    "integration_key": "string"
  },
  "vehicle": {
    "id": "string",
    "integration_key": "string",
    "registration": "string",
    "fleet_number": "string",
    "description": null,
    "odometer": 0.0
  }
}
```