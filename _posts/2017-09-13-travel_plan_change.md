---
layout: default
title:  "Travel Plan Change"
date:   2017-09-13 13:40:00 +0200
categories: loads integration
excerpt: The stop requires you to specify the location id instead of the shipping address id
---

# Travel Plan Change - 2017-09-13

It makes more sense in the long term to have the location integration key specified on the stop instead of the shipping address integration key. This is due to the fact that a mix of pickups and dropoffs can be allocated to a stop with different shipping addresses however they will be linked to the same location. We have made this explicit to avoid any confusion

## Compatibility

The change is backward compatible but will become obsolete after 60 days. The change will need to be made on your integrations within 60 days to prevent service interruption.

## Changes

The changes affect the following areas

### Travel Plan Stop

When implementing the change please ensure that you change the value you map to `location_integration_key`. It is not enough to simply change the name of the property since it must reference a location instead of a shipping address.

An optional `address` field has been added to the stop which will allow you to capture the physical address of the stop. The physical addresses may be different to the business shipping address. This property will allow you to capture both if required.

#### Before

```
{
	...
	"load": {
		"travel_plan": {
			"stops": [{
				"shipping_address_integration_key": "..."
			}]
		}
	}
	...
}
```

#### After

```
{
	...
	"load": {
		"travel_plan": {
			"stops": [{
				"location_integration_key": "...",
				"address": {
					...
				}
			}]
		}
	}
	...
}
```