# Webhook Payloads

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
    }
  },
  "when": "2017-05-15T13:55:11.1354101Z",
  "where": [
    0.0,
    0.0
  ]
}
```

## Stop Arrived `load.stop.arrived`
```
{
  "when": "2017-05-15T13:55:11.1344096Z",
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
    }
  },
  "travel_plan_poi_id": "string",
  "integration_key": "string"
}
```

## Stop Departed `load.stop.departed`
```
{
  "when": "2017-05-15T13:55:11.1354101Z",
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
    }
  },
  "travel_plan_poi_id": "string",
  "integration_key": "string"
}
```

## Dropoff Started `load.dropoff.started`
```
{
  "when": "2017-05-15T13:55:11.1364093Z",
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
    }
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
    "due_at": "2017-05-15T13:55:11.1374107Z",
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

## Dropoff Completed `load.dropoff.completed`
```
{
  "when": "2017-05-15T13:55:11.1384104Z",
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
    }
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
    "due_at": "2017-05-15T13:55:11.1384104Z",
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
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
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
    ]
  }
}
```

## Pickup Started `load.pickup.started`
```
{
  "when": "2017-05-15T13:55:11.1384104Z",
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
    }
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
    "due_at": "2017-05-15T13:55:11.1394109Z",
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

## Pickup Completed `load.pickup.completed`
```
{
  "when": "2017-05-15T13:55:11.1394109Z",
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
    }
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
    "due_at": "2017-05-15T13:55:11.1404105Z",
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
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
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
    ]
  }
}
```

## Rest Stop `rest_stop`
```
{
  "when": "2017-05-15T13:55:11.1414123Z",
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
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
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
    ]
  }
}
```

## Border Crossing `border_crossing`
```
{
  "when": "2017-05-15T13:55:11.1404105Z",
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
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
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
  "when": "2017-05-15T13:55:11.1404105Z",
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
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
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
  "when": "2017-05-15T13:55:11.1424116Z",
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
    }
  },
  "asset_id": "string",
  "meter_reading": 0.0,
  "integration_key": null,
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
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
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
    ]
  }
}
```

## Weighbridge `weighbridge`
```
{
  "when": "2017-05-15T13:55:11.1424116Z",
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
        "asset_identifier": {
          "type": "string",
          "identifier": "string"
        },
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