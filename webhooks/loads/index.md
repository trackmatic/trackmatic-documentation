# Webhook Payloads
## Border Crossing `border_crossing`
```
{
  "when": "2017-10-20T14:08:45.3915778Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
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
    "fleet_number": "string"
  }
}
```
## Border Crossing Failed `border_crossing.failed`
```
{
  "when": "2017-10-20T14:08:45.3925783Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
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
    "fleet_number": "string"
  }
}
```
## Breakdown `breakdown`
```
{
  "when": "2017-10-20T14:08:45.399576Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
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
    "fleet_number": "string"
  }
}
```
## Dropoff Completed `load.dropoff.completed`
```
{
  "when": "2017-10-20T14:08:45.38958Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": null,
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
    "due_at": "2017-10-20T14:08:45.38958Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
  }
}
```
## Dropoff Failed `load.dropoff.failed`
```
{
  "when": "2017-10-20T14:08:45.38958Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": null,
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
    "due_at": "2017-10-20T14:08:45.3905797Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
  },
  "failure_reason": null
}
```
## Dropoff Started `load.dropoff.started`
```
{
  "when": "2017-10-20T14:08:45.388403Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": null,
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
    "due_at": "2017-10-20T14:08:45.38958Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
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
}
```
## Fuel Stop Completed `fuel_stop.completed`
```
{
  "when": "2017-10-20T14:08:45.3935788Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
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
    "fleet_number": "string"
  }
}
```
## Fuel Stop Failed `fuel_stop.failed`
```
{
  "when": "2017-10-20T14:08:45.3945801Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
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
    "fleet_number": "string"
  }
}
```
## Fuel Stop Started `fuel_stop.started`
```
{
  "when": "2017-10-20T14:08:45.3925783Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
    "fleet_number": "string"
  }
}
```
## Load Activated `load.activated`
```
{
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "when": "2017-10-20T14:08:45.3879054Z",
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
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "when": "2017-10-20T14:08:45.388403Z",
  "reason": "string"
}
```
## Load Claimed `load.claimed`
```
{
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "when": "2017-10-20T14:08:45.4005765Z",
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
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "force_closed": false,
  "when": "2017-10-20T14:08:45.3879054Z",
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
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "when": "2017-10-20T14:08:45.388403Z"
}
```
## Load Released `load.released`
```
{
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "when": "2017-10-20T14:08:45.4005765Z",
  "where": [
    0.0,
    0.0
  ]
}
```
## Odometer `odometer`
```
{
  "when": "2017-10-20T14:08:45.3965799Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
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
    "fleet_number": "string"
  }
}
```
## Odometer Failed `odometer.failed`
```
{
  "when": "2017-10-20T14:08:45.3965799Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
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
    "fleet_number": "string"
  }
}
```
## Off Route `off_route`
```
{
  "when": "2017-10-20T14:08:45.399576Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  }
}
```
## Pickup Completed `load.pickup.completed`
```
{
  "when": "2017-10-20T14:08:45.3915778Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": null,
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
    "due_at": "2017-10-20T14:08:45.3915778Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
  }
}
```
## Pickup Failed `load.pickup.failed`
```
{
  "when": "2017-10-20T14:08:45.3915778Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": null,
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
    "due_at": "2017-10-20T14:08:45.3915778Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
  },
  "failure_reason": null
}
```
## Pickup Started `load.pickup.started`
```
{
  "when": "2017-10-20T14:08:45.3905797Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "integration_key": "string",
    "reference": null,
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
    "due_at": "2017-10-20T14:08:45.3905797Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
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
}
```
## Rest Stop Completed `rest_stop.completed`
```
{
  "when": "2017-10-20T14:08:45.3955806Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
    "e_documents": []
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
    "fleet_number": "string"
  },
  "reference_number": null
}
```
## Rest Stop Failed `rest_stop.failed`
```
{
  "when": "2017-10-20T14:08:45.3955806Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
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
    "fleet_number": "string"
  },
  "reference_number": null
}
```
## Rest Stop Started `rest_stop.started`
```
{
  "when": "2017-10-20T14:08:45.3945801Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
    "fleet_number": "string"
  },
  "reference_number": "string"
}
```
## Stop Arrived `load.stop.arrived`
```
{
  "when": "2017-10-20T14:08:45.3869045Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "travel_plan_poi_id": "string",
  "integration_key": "string"
}
```
## Stop Departed `load.stop.departed`
```
{
  "when": "2017-10-20T14:08:45.3874058Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
  },
  "travel_plan_poi_id": "string",
  "integration_key": "string"
}
```
## Weighbridge Completed `weighbridge.completed`
```
{
  "when": "2017-10-20T14:08:45.3975767Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
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
    "fleet_number": "string"
  }
}
```
## Weighbridge Failed `weighbridge.failed`
```
{
  "when": "2017-10-20T14:08:45.3985764Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
        "received_by_driver": false,
        "valid_proof_of_payment_provided": false,
        "customer_reference": "string",
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
    "e_documents": []
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
    "fleet_number": "string"
  }
}
```
## Weighbridge Started `weighbridge.started`
```
{
  "when": "2017-10-20T14:08:45.3975767Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "integration_key": null,
    "requested_date": "0001-01-01T00:00:00",
    "reference": null,
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
        "fleet_number": "string"
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
    "type": null
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
    "fleet_number": "string"
  }
}
```