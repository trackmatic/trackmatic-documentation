---
layout: default
title:  "Delayed Requirement"
date:   2018-02-07 08:00:00 +0200
categories: loads integration
excerpt: Introducing delayed requirements
---

# Delayed Requirements - 2018-02-07

A new requirement has been introduced which will allow you to request the driver to capture the reason for any delays experienced while executing a given activity.

The requirement is specified in the same way as other requirements and allows you to provide a list of reasons for the delay. 

For example:

```
"requirements": {
	"success_sequence": [
		"delay"
	],
	"failure_sequence": [],
	"signatures": [],
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
	"delays": [
		{
			"reasons": [
				"Reason 1",
				"Reason 2",
				"Reason 3"
			],
			"integration_key": "delay",
			"label": "Where there any delays?",
			"is_optional": false
		}
	]
}
```