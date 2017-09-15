---
layout: default
title:  "Remove Asset Identifier"
date:   2017-09-13 13:40:00 +0200
categories: loads integration
excerpt: The asset identifier element has been replaced with more specific properties
---

# Remove Asset Identifier - 2017-09-15

Previously there was an `asset_identifier` property on the odometer reading requirement and activity. In order to make the intent of this feature more explicit it has been replaced with two independent properties namely `asset_integration_key` and `asset_type`

Both fields are optional and only one must be supplied for a single instance. If the asset type is supplied the system will ensure that the driver selects or scans an asset for the supplied type. If the asset integration key is supplied the system will ensure that the driver selected the specific asset.

## Compatibility

The change is backward compatible but will become obsolete after 60 days. The change will need to be made on your integrations within 60 days to prevent service interruption.

## Changes

The changes affect the following areas

### Odometer Readings Requirement

#### Before

```
{
	...
	"odometer_readings": [{
		"asset_identifier": {
			"type": "...",
			"identifier" "..."
		}
	}]
	...
}
```

#### After

```
{
	...
	"odometer_readings": [{
		"asset_integration_key": "...",
		"asset_type": "..."
	}]
	...
}
```

### Odometer Readings Activity

#### Before

```
{
	...
	"planned_activities": {
		"odometer_readings": [{
			"asset_identifier": {
				"type": "...",
				"identifier" "..."
			}
		}]
	}
	...
}
```

#### After

```
{
	...
	"planned_activities": {
		"odometer_readings": [{
			"asset_type": "...",
			"asset_integration_key": "..."
		}]
	}
	...
}
```