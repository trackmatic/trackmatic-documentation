---
layout: default
title:  "Custom Activities"
date:   2018-02-07 08:00:00 +0200
categories: loads integration
excerpt: Introducing custom activities
---

# Custom Activities - 2018-09-27

Custom activities were introduced to allow requirements to be executed without any other steps.
To plan a custom activity you must specify the activity under planned activities as per below

```
"planned_activities": {
    "rest_stops": [],
    "weighbridges": [],
    "fuel_stops": [],
    "border_crossings": [],
    "pallet_drops": [],
    "fatigue_assessments": [],
    "odometer_readings": [],
    "release_loads": [],
    "multi_pickups": [],
    "multi_dropoffs": [],
    "timed_tasks": [],
    "custom_activities": [
      {
        "name": "Custom Activity",
        "description": "My activity",
        "duration": "00:10:00",
        "integration_key": "custom_activity_1",
        "requirements": {
          "success_sequence": null,
          "failure_sequence": null,
          "signatures": null,
          "cash_on_deliveries": null,
          "document_scans": null,
          "images": null,
          "service_ratings": null,
          "odometer_readings": null,
          "pallet_tansfers": null,
          "proof_of_deliveries": null,
          "weighbridge_readings": null,
          "pallet_drops": null,
          "e_documents": null,
          "forms": null,
          "delays": []
        }
      }
    ]
  }
```

Then you can plan it into the travel plan, the same as any other activity, as per below

```
"travel_plan": {
	"stops": [
		{
			"integration_key": "poi2",
			"description": "Pickup 1",
			"path_to": null,
			"location_integration_key": "geofence_refactor1",
			"due_time": null,
			"time_at_stop": null,
			"activities": [
				{
					"related_integration_key": "custom_activity_1",
					"type": "custom_activity",
					"name": "My activity",
					"description": "",
					"duration": "00:30:00"					
				}
			],
			"address": null
		}
	],
	...
}
```