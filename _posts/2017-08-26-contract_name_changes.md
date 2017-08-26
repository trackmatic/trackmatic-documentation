---
layout: default
title:  "Contract Name Changes"
date:   2017-08-26 09:00:00 +0200
categories: loads integration
---

# Loads Integration Migration

We have made some name changes in order to align the integration API with the rest of the system as it grows.

There are a few areas of the [load import]({{'/rest/loads/integration/open-api#operation/Loads_Import' | prepend: site.github.url}}) request which have been affected.

- "Point of interest" has been changed to "Stop"
- "Geofence" has been changed to "Location"

The changes affect the following areas

## Geofences collection

`geofences` collection on the route element has been changed tp `locations`

### Before

```
{
	...
	"geofences": [...]
	...
}
```

### After

```
{
	...
	"locations": [...]
	...
}
```

## Geofence reference in Shipping Address

Within the shipping address there was a a property named `geofence_integration_key`, this has been changed to `location_integration_key`

### Before

```
{
	...
	"shipping_addresses": [{
		...
		"geofence_integration_key": "..."
		...
	}]
	...
}
```

### After

```
{
	...
	"shipping_addresses": [{
		...
		"location_integration_key": "..."
		...
	}]
	...
}
```

## Data Ownership

`geofence' property in the data ownership element has been changed to `location`

### Before

```
{
	...
	"data_ownership": {
		...
		"geofence": { ... }
		...
	}
	...
}
```

### After

```
{
	...
	"data_ownership": {
		...
		"location": { ... }
		...
	}
	...
}
```

## Points of interest

The `points_of_interest` property on the travel plan has been renamed to `stops`

### Before

```
{
	...
	"load": {
		...
		"travel_plan": {
			"points_of_interest": [ ... ]
		}
		...
	}
	...
}
```

### After

```
{
	...
	"load": {
		...
		"travel_plan": {
			"stops": [ ... ]
		}
		...
	}
	...
}
```

## Compatibility

The change is backward compatible but will become obsolete after 60 days. The change will need to made on your integrations within 60 days to prevent service interruption.