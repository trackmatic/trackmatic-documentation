---
layout: default
title:  "Timed Tasks"
date:   2018-02-19 20:00:00 +0200
categories: loads integration
excerpt: Introducing requirement conditions
---

# Requirement Conditions - 2018-02-19

Requirement conditions have been introduced to allow you to control when the driver should execute a given requirement. Currently we support 2 requirement conditions namely `confirmations` and `late_arrivals`. Conditions can be used on any requirement.

## Confirmations

A confirmation condition allows you to specify a question to ask a driver, if the answer the driver answers yes to the question then the requirement need to be executed, if the answer is no then the requirement will be skipped.

You have the ability to specify the question as well as the confirm text and reject text.

```
{
	"conditions": {
		"confirmations": [{
			"question": "string",
			"confirm_text": "string",
			"reject_text": "string"
		}]
	}
}
```

For example, if the driver was delayed and you want him to provide a reason for being late only if there were delays, you could model this as follows:

```
{
	"requirements": {
		"delays": [{
			"reasons": ["Traffic", "Had to wait for a bay", "I arrived late"],
			"integration_key": "delay",
			"label": "What caused the delays?",
			"conditions": {
				"confirmations": [{
					"question": "Where there any delays?",
					"confirm_text": "Yes",
					"reject_text": "No"
				}]
			}
		}]
	}
}
```

## Late Arrivals

The late arrival condition allows you to specify that a requirement which is only fulfilled if the driver arrived late and outside of the supplied threshold.

```
{
	"conditions": {
		"late_arrivals": [{
			"threshold": "00:00:00"
		}]
	}
}
```


For example, if you wanted the driver to provide a reason for arriving at the stop late but only if he arrived 30 mins after the planned, then you could model this as follows:

```
{
	"requirements": {
		"delays": [{
			"reasons": ["Traffic", "Breakdown", "Delayed at last stop"],
			"integration_key": "delay",
			"label": "Why were you late?",
			"conditions": {
				"late_arrivals": [{
					"threshold": "00:30:00"
				}]
			}
		}]
	}
}
```

Requirements have been also been added to stops to support the executing a requirement on arrival at a stop. This is done via the travel plan as follows:

```
{
	"load": {
		"travel_plan": {
			"stops": [{
				"requirements": {
					"delays": [{
						"reasons": ["Traffic", "Breakdown", "Delayed at last stop"],
						"integration_key": "delay",
						"label": "Why were you late?",
						"conditions": {
							"late_arrivals": [{
								"threshold": "00:30:00"
							}]
						}
					}]
				}
			}]
		}
	}
}
```