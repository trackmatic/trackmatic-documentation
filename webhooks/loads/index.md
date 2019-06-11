#Webhooks Payloads
## Actions Dropoff Attempted `load.actiondropoff.attempted`
```
{
  "when": "2019-06-11T14:06:34.7899069Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7909035Z",
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
      }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7909035Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7919365Z",
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
      }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7899069Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7899069Z",
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
      }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7929065Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "pickups": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7929065Z",
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
      }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7939388Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "pickups": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7939388Z",
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
      }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7919365Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "pickups": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7919365Z",
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
      }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7739045Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
    "description": null
  }
}
```
## Border Crossing Failed `border_crossing.failed`
```
{
  "when": "2019-06-11T14:06:34.7749065Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
    "description": null
  }
}
```
## Breakdown `breakdown`
```
{
  "when": "2019-06-11T14:06:34.7859008Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
    "description": null
  }
}
```
## Custom Activity Completed `custom_activity.completed`
```
{
  "when": "2019-06-11T14:06:34.7879012Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7879012Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7669063Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
    "reference": "string",
    "pickup_ids": [
      "string"
    ],
    "dropoff_ids": [
      "string"
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
    }
  },
  "dropoff": {
    "integration_key": "string",
    "due_at": "2019-06-11T14:06:34.7669063Z",
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
    }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7709068Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
    "reference": "string",
    "pickup_ids": [
      "string"
    ],
    "dropoff_ids": [
      "string"
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
    }
  },
  "dropoff": {
    "integration_key": "string",
    "due_at": "2019-06-11T14:06:34.7719074Z",
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
    }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7669063Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
    "reference": "string",
    "pickup_ids": [
      "string"
    ],
    "dropoff_ids": [
      "string"
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
    }
  },
  "dropoff": {
    "integration_key": "string",
    "due_at": "2019-06-11T14:06:34.7669063Z",
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
    }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.775903Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
    "description": null
  }
}
```
## Fuel Stop Failed `fuel_stop.failed`
```
{
  "when": "2019-06-11T14:06:34.7769021Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
    "description": null
  }
}
```
## Fuel Stop Started `fuel_stop.started`
```
{
  "when": "2019-06-11T14:06:34.7749065Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
    "description": null
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7629106Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7659064Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7859008Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7659064Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7659064Z"
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
    "start": "2019-06-11T14:06:34.7649068Z",
    "end": "2019-06-11T14:06:34.7659064Z",
    "pois": [
      {
        "travel_plan_poi_id": "String",
        "due_time": "2019-06-11T14:06:34.7659064Z",
        "geofence_id": "string",
        "geofence_name": "string"
      }
    ]
  },
  "consignments": [
    {
      "id": "string",
      "cargo_type": "string",
      "integration_key": "string",
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "pickups": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7649068Z",
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7639071Z",
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
      }
    }
  ],
  "when": "2019-06-11T14:06:34.7639071Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7869018Z",
  "where": [
    0.0,
    0.0
  ]
}
```
## Multi Dropoff Completed `load.multidropoff.completed`
```
{
  "when": "2019-06-11T14:06:34.7679065Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7689079Z",
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
      }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
          "qty": 0,
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
  "is_complete": false
}
```
## Multi Dropoff Failed `load.multidropoff.failed`
```
{
  "when": "2019-06-11T14:06:34.7689079Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7699063Z",
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
      }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
          "qty": 0,
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
  "when": "2019-06-11T14:06:34.7669063Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7679065Z",
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
      }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7699063Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "pickups": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7699063Z",
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
      }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7689079Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "dropoffs": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7699063Z",
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
      }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
          "qty": 0,
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
  "when": "2019-06-11T14:06:34.7679065Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
      "reference": "string",
      "pickup_ids": [
        "string"
      ],
      "dropoff_ids": [
        "string"
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
      }
    }
  ],
  "pickups": [
    {
      "integration_key": "string",
      "due_at": "2019-06-11T14:06:34.7679065Z",
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
      }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7799009Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
    "description": null
  }
}
```
## Odometer Failed `odometer.failed`
```
{
  "when": "2019-06-11T14:06:34.7819026Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
    "description": null
  }
}
```
## Off Route `off_route`
```
{
  "when": "2019-06-11T14:06:34.7859008Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7719074Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
    "reference": "string",
    "pickup_ids": [
      "string"
    ],
    "dropoff_ids": [
      "string"
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
    }
  },
  "pickup": {
    "integration_key": "string",
    "due_at": "2019-06-11T14:06:34.7729059Z",
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
    }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7729059Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
    "reference": "string",
    "pickup_ids": [
      "string"
    ],
    "dropoff_ids": [
      "string"
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
    }
  },
  "pickup": {
    "integration_key": "string",
    "due_at": "2019-06-11T14:06:34.7729059Z",
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
    }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7719074Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
    "reference": "string",
    "pickup_ids": [
      "string"
    ],
    "dropoff_ids": [
      "string"
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
    }
  },
  "pickup": {
    "integration_key": "string",
    "due_at": "2019-06-11T14:06:34.7719074Z",
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
    }
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
## Rest Stop Completed `rest_stop.completed`
```
{
  "when": "2019-06-11T14:06:34.7789353Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
    "description": null
  },
  "reference_number": null
}
```
## Rest Stop Failed `rest_stop.failed`
```
{
  "when": "2019-06-11T14:06:34.7799009Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
    "description": null
  },
  "reference_number": null
}
```
## Rest Stop Started `rest_stop.started`
```
{
  "when": "2019-06-11T14:06:34.777942Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
    "description": null
  },
  "reference_number": "string"
}
```
## Stop Arrived `load.stop.arrived`
```
{
  "when": "2019-06-11T14:06:34.7619117Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7629106Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7829058Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7819026Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
  "when": "2019-06-11T14:06:34.7869018Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7879012Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7869018Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
  "when": "2019-06-11T14:06:34.7839042Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
    "description": null
  }
}
```
## Weighbridge Failed `weighbridge.failed`
```
{
  "when": "2019-06-11T14:06:34.7849013Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
            "completed_on": "2019-06-11T14:06:34.7589134Z"
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
    "description": null
  }
}
```
## Weighbridge Started `weighbridge.started`
```
{
  "when": "2019-06-11T14:06:34.7829058Z",
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
      "vehicle": {
        "id": "string",
        "integration_key": "string",
        "registration": "string",
        "fleet_number": "string",
        "description": "string"
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
    "description": null
  }
}
```