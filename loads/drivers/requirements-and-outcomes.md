# Requirements & Outcomes

Requirements and outcomes and the building blocks of an activity. The requirements are used to instruct the driver what information to gather once they have completed any activity. The outcomes are what are sent back to the server and hold the data captured by the driver. There are a number of reuqirements and associated outcomes. The remainder of this section will detail each one.

## Requirement Sequence

The order in which requirements should be fulfilled is defined by the `execution_sequence` property on the activity. The `execution_sequence` sequence contains a list of `integration_keys` correlates to the `integration_key` property on each requirements. The `integration_key` is a unique identifier for each requirement within the context of an activity.

## Outcome Status

When completeing an outcome it can result in one of the following statuses:

|Status|Description|
|------|-----------|
|success|The outcome was successfully captured|
|skipped|The outcome was intentionally skipped by the user. This is only possible if the `is_optional` field is marked as true. A reason is requirement to be provided in the `status_reason` field in this case|
|failed|The outcome could not be captured for reasons outside of the drivers control. A reason is requirement to be provided in the `status_reason` field in this case|

## Common Outcome Properties

|Field|Description|
|-----|-----------|
|label|The display value of the requirement, this would typically displayed on screen to the driver|
|is_optional|When `true` the driver should be allowed to skip the requirement|

## Odometers

The odometer requirement instructs the driver to capture an odometer reading for the specified asset. 

The `asset_id` field describes which asset the odometer value should be captured for. The asset id field can be used to look up additional asset information in the `assets` tag of the allocation on a load.

The `asset` object appears as follows:

```
{
    "id": "string",
    "reference": "string",
    "integration_key": "string",
    "fleet_number": "string",
    "type": "string", [trailer, vehicle, forklift]
    "odometer": {
        "meter_type": "string", [distance or hours]
        "value": 0
    }
}
```

### Requirement

```
{
    "validate": true,
    "asset_id": "string",
    "integration_key": "string",
    "label": "string",
    "is_optional": true
}
```

### Outcome

The asset odometer can be measure in `hours` or `distance`. The `meter_type` from the asset should be used to populate the associated outcome `meter_type` property.

```
{
    "meter_type": "Distance",
    "value": "string",
    "asset_identifier": {
        "type": "AssetId",
        "identifier": "string"
    },
    "integration_key": "string",
    "status": "Success",
    "status_reason": "string"
}
```

|Field|Description|
|-----|-----------|
|validate|When `true` the captured odometer value must be validated against the current odometer value on the asset|
|asset_id|The asset id which the odometer reading is being captured for|
