# Webhook Payloads

## Load Activated `load.activated`
```
{
  "load": {
    "id": null,
    "reference": null,
    "requested_date": "0001-01-01T00:00:00",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "reference": "string"
      },
      "vehicle": {
        "id": "string",
        "reference": "string",
        "registration": "string",
        "fleet_number": "string"
      },
      "assets": [
        {
          "reference": "string",
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
    }
  },
  "when": "2017-04-03T14:45:42.0145849Z",
  "where": [
    0.0,
    0.0
  ]
}
```

## Stop Arrived `load.stop.arrived`
```
{
  "when": "2017-04-03T14:45:42.0135815Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "reference": null,
    "requested_date": "0001-01-01T00:00:00",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "reference": "string"
      },
      "vehicle": {
        "id": "string",
        "reference": "string",
        "registration": "string",
        "fleet_number": "string"
      },
      "assets": [
        {
          "reference": "string",
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
    }
  },
  "travel_plan_poi_id": "string",
  "reference": "string"
}
```

## Stop Departed `load.stop.departed`
```
{
  "when": "2017-04-03T14:45:42.0145849Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "reference": null,
    "requested_date": "0001-01-01T00:00:00",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "reference": "string"
      },
      "vehicle": {
        "id": "string",
        "reference": "string",
        "registration": "string",
        "fleet_number": "string"
      },
      "assets": [
        {
          "reference": "string",
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
    }
  },
  "travel_plan_poi_id": "string",
  "reference": "string"
}
```

## Dropoff Started `load.dropoff.started`
```
{
  "when": "2017-04-03T14:45:42.0145849Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "reference": null,
    "requested_date": "0001-01-01T00:00:00",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "reference": "string"
      },
      "vehicle": {
        "id": "string",
        "reference": "string",
        "registration": "string",
        "fleet_number": "string"
      },
      "assets": [
        {
          "reference": "string",
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
    }
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "reference": "string",
    "consignor": {
      "entity_id": "string",
      "name": "string",
      "reference": "string"
    },
    "consignee": {
      "entity_id": "string",
      "name": "string",
      "reference": "string"
    }
  },
  "dropoff": {
    "reference": "string",
    "due_at": "2017-04-03T14:45:42.0145849Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
    },
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "reference": "string"
    },
    "shipping_address": {
      "reference": "string",
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
}
```

## Dropoff Completed `load.dropoff.completed`
```
{
  "when": "2017-04-03T14:45:42.0155854Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "reference": null,
    "requested_date": "0001-01-01T00:00:00",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "reference": "string"
      },
      "vehicle": {
        "id": "string",
        "reference": "string",
        "registration": "string",
        "fleet_number": "string"
      },
      "assets": [
        {
          "reference": "string",
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
    }
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "reference": "string",
    "consignor": {
      "entity_id": "string",
      "name": "string",
      "reference": "string"
    },
    "consignee": {
      "entity_id": "string",
      "name": "string",
      "reference": "string"
    }
  },
  "dropoff": {
    "reference": "string",
    "due_at": "2017-04-03T14:45:42.0155854Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
    },
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "reference": "string"
    },
    "shipping_address": {
      "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "reference": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  }
}
```

## Pickup Started `load.pickup.started`
```
{
  "when": "2017-04-03T14:45:42.0155854Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "reference": null,
    "requested_date": "0001-01-01T00:00:00",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "reference": "string"
      },
      "vehicle": {
        "id": "string",
        "reference": "string",
        "registration": "string",
        "fleet_number": "string"
      },
      "assets": [
        {
          "reference": "string",
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
    }
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "reference": "string",
    "consignor": {
      "entity_id": "string",
      "name": "string",
      "reference": "string"
    },
    "consignee": {
      "entity_id": "string",
      "name": "string",
      "reference": "string"
    }
  },
  "pickup": {
    "reference": "string",
    "due_at": "2017-04-03T14:45:42.0155854Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
    },
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "reference": "string"
    },
    "shipping_address": {
      "reference": "string",
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
}
```

## Pickup Completed `load.pickup.completed`
```
{
  "when": "2017-04-03T14:45:42.0165674Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "reference": null,
    "requested_date": "0001-01-01T00:00:00",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "reference": "string"
      },
      "vehicle": {
        "id": "string",
        "reference": "string",
        "registration": "string",
        "fleet_number": "string"
      },
      "assets": [
        {
          "reference": "string",
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
    }
  },
  "consignment": {
    "id": "string",
    "cargo_type": "string",
    "reference": "string",
    "consignor": {
      "entity_id": "string",
      "name": "string",
      "reference": "string"
    },
    "consignee": {
      "entity_id": "string",
      "name": "string",
      "reference": "string"
    }
  },
  "pickup": {
    "reference": "string",
    "due_at": "2017-04-03T14:45:42.0165674Z",
    "quantity": {
      "value": 0.0,
      "units": "string"
    },
    "maximum_service_time": "00:00:00",
    "entity": {
      "entity_id": "string",
      "name": "string",
      "reference": "string"
    },
    "shipping_address": {
      "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "reference": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  }
}
```

## Rest Stop `rest_stop`
```
{
  "when": "2017-04-03T14:45:42.0175667Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "reference": null,
    "requested_date": "0001-01-01T00:00:00",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "reference": "string"
      },
      "vehicle": {
        "id": "string",
        "reference": "string",
        "registration": "string",
        "fleet_number": "string"
      },
      "assets": [
        {
          "reference": "string",
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
    }
  },
  "feeling": "string",
  "planned_duration": "00:00:00",
  "comments": "string",
  "reason": "string",
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "reference": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  }
}
```

## Border Crossing `border_crossing`
```
{
  "when": "2017-04-03T14:45:42.0165674Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "reference": null,
    "requested_date": "0001-01-01T00:00:00",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "reference": "string"
      },
      "vehicle": {
        "id": "string",
        "reference": "string",
        "registration": "string",
        "fleet_number": "string"
      },
      "assets": [
        {
          "reference": "string",
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
    }
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "reference": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "country": "string",
  "name": "string",
  "money_order_number": "string",
  "border_permit_number": "string"
}
```

## Fuel Stop `fuel_stop`
```
{
  "when": "2017-04-03T14:45:42.0165674Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "reference": null,
    "requested_date": "0001-01-01T00:00:00",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "reference": "string"
      },
      "vehicle": {
        "id": "string",
        "reference": "string",
        "registration": "string",
        "fleet_number": "string"
      },
      "assets": [
        {
          "reference": "string",
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
    }
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "reference": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "authorized_location": false,
  "transaction_reference": "string",
  "transactions": [
    {
      "litres": 0.0,
      "cost": 0.0,
      "full_tank": false,
      "asset_id": "string",
      "odometer_reading": 0.0
    }
  ]
}
```

## Odometer `odometer`
```
{
  "when": "2017-04-03T14:45:42.0175667Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "reference": null,
    "requested_date": "0001-01-01T00:00:00",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "reference": "string"
      },
      "vehicle": {
        "id": "string",
        "reference": "string",
        "registration": "string",
        "fleet_number": "string"
      },
      "assets": [
        {
          "reference": "string",
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
    }
  },
  "asset_id": "string",
  "meter_reading": 0.0,
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "reference": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  }
}
```

## Weighbridge `weighbridge`
```
{
  "when": "2017-04-03T14:45:42.0175667Z",
  "where": [
    0.0,
    0.0
  ],
  "load": {
    "id": null,
    "reference": null,
    "requested_date": "0001-01-01T00:00:00",
    "allocation": {
      "driver": {
        "id": "string",
        "name": "string",
        "reference": "string"
      },
      "vehicle": {
        "id": "string",
        "reference": "string",
        "registration": "string",
        "fleet_number": "string"
      },
      "assets": [
        {
          "reference": "string",
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
    }
  },
  "outcomes": {
    "signatures": [
      {
        "image_url": "string",
        "name": "string",
        "comment": "string",
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
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
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "service_ratings": [
      {
        "type": "string",
        "value": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "odometer_readings": [
      {
        "meter_type": "string",
        "value": "string",
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "pallet_transfers": [
      {
        "qty_transfered": 0,
        "transfer_reference": "string",
        "comment": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "proof_of_deliveries": [
      {
        "document_references": [
          "string"
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "weights": [
      {
        "unit": "string",
        "value": "string",
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ],
    "forms": [
      {
        "fields": [
          {
            "reference": "string",
            "label": "string",
            "value": "string",
            "data_type": "string"
          }
        ],
        "reference": "string",
        "status": "string",
        "status_reason": "string"
      }
    ]
  },
  "name": "string",
  "failed": false,
  "failure_reason": "string",
  "impounded": false,
  "file_names": [
    "string"
  ]
}
```

