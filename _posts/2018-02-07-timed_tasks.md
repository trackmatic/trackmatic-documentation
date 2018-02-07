---
layout: default
title:  "Timed Tasks"
date:   2018-02-07 08:00:00 +0200
categories: loads integration
excerpt: Introducing timed tasks
---

# Timed Tasks - 2018-02-07

Timed tasks have been introduced to the system which will allow you to plan custom timed tasks for the driver to execute at a stop. The timed task works in the same was as most other timed activities, such as Pickups and Dropoffs, but is not related to any other business specific info.

To plan a timed task you must specify the activity under planned activities as per below

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
    "timed_tasks": [
      {
        "name": "Timed Task",
        "description": "My Timed Task",
        "duration": "00:10:00",
        "integration_key": "timed_task_1",
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
        },
        "timer_type": "up"
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
					"related_integration_key": "timed_task_1",
					"type": "timed_task",
					"name": "My Timed Task",
					"description": "",
					"duration": "00:30:00",
					"timer_type": null
				}
			],
			"address": null
		}
	],
	...
}
```