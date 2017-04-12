# Requirements & Outcomes

Requirements and outcomes and the building blocks of an activity. The requirements are used to instruct the driver what information to gather once they have completed any activity. The outcomes are what are sent back to the server and hold the data captured by the driver. There are a number of reuqirements and associated outcomes. The remainder of this section will detail each one.

- [Odometers](#odometers)
- [Forms](#forms)
- [Service Ratings](#service-ratings)
- [Weights](#weights)
- [Images](#images)

### Execution Sequence

The order in which requirements should be fulfilled is defined by the `execution_sequence` property on the activity. The `execution_sequence` sequence contains a list of `integration_keys` correlates to the `integration_key` property on each requirements. The `integration_key` is a unique identifier for each requirement within the context of an activity.

### Common Requirement Properties

|Field|Description|
|-----|-----------|
|label|The display value of the requirement, this would typically displayed on screen to the driver|
|is_optional|When `true` the driver should be allowed to skip the requirement|
|integration_key|The `integration_key` identifier provided by the requirement|


### Outcome Status

When completing an outcome a status must be set to one of the following:

|Status|Description|
|------|-----------|
|success|The outcome was successfully captured|
|skipped|The outcome was intentionally skipped by the user. This is only possible if the `is_optional` field is marked as true. A reason is requirement to be provided in the `status_reason` field in this case|
|failed|The outcome could not be captured for reasons outside of the drivers control. A reason is requirement to be provided in the `status_reason` field in this case|

## Odometers

The odometer requirement instructs the driver to capture an odometer reading for the specified asset. 

The `asset_id` field describes which asset the odometer value should be captured for. The asset id field can be used to look up additional asset information in the `assets` tag of the allocation on a load.

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

|Field|Description|
|-----|-----------|
|validate|When `true` the captured odometer value must be validated against the current odometer value on the asset|
|asset_id|The asset id which the odometer reading is being captured for|

### Outcome

The asset odometer can be measure in `hours` or `distance`. The `meter_type` from the asset should be used to populate the associated outcome `meter_type` property of the outcome.

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
|meter_type|Must be either `distance` or `hours` and can be set from the original asset|
|asset_identifier|The value which identifies the asset. The type can be either `asset_id`, `registration` or `integration_key` and shoud be set based on the type of barcode which is scanned|
|value|The captured odometer reading|

## Forms

The forms requirement prompts the driver to fill in the defined form. The requirement should be used as meta data to dynamically construct the form.

### Requirement

A form consists of one or more fields. Each field has an `integration_key` property which uniquely identifies the field and is used to correlate the value within the source system. Each 

```
{
  "fields": [
    {
      "data_type": "string",
      "label": "string",
      "integration_key": "string",
      "options": [
        "string"
      ],
      "required": true,
      "regex": "string",
      "range": [
        "string"
      ]
    }
  ],
  "integration_key": "string",
  "label": "string",
  "is_optional": true
}
```

|Property|Description|
|--------|-----------|
|data_type|Describes the data-type to be captured. Can be one of `date`, `number`, `text` or `boolean`|
|options|If populated a drop down list should be rendered which contains the values provided in options|
|required|When `true` the field is required|
|regex|When provided the input should be validated against the regular expression|
|range|When provided the entered value should be bewteen the provided values. The array will only ever have 2 elements and only applies to dates and numbers|

### Outcome

```
{
  "fields": [
    {
      "integration_key": "string",
      "value": "string",
      "label": "string",
      "data_type": "Text"
    }
  ],
  "integration_key": "string",
  "status": "Success",
  "status_reason": "string"
}
```

|Property|Description|
|--------|-----------|
|data_type|Describes the data-type to be captured. Can be one of `date`, `number`, `text` or `boolean`. Must be the same as the original requirement|
|value|The captured value in the string representation of the `data_type`|

## Service Ratings

Service ratings provide a way to capture questionaire information from the driver and/or the customer. Currently the system specifies 3 service rating types.

### Requirement

```
{
  "type": "string",
  "integration_key": "string",
  "label": "string",
  "is_optional": true
}
```

|Type|Description|
|----|-----------|
|star|Should display 5 stars. 1 is the lowest while 5 is the highest|
|smiley|Should display 3 smiley faces. Dissatisfied (1), neutral (2) and satisfied (3)|
|simple|Should display thumbs down (1) and thumbs up (2)|

### Outcome

```
{
  "type": "string",
  "value": "string",
  "comment": "string",
  "integration_key": "string",
  "status": "Success",
  "status_reason": "string"
}
```

|Property|Description|
|----|-----------|
|value|The numeric value representing the rating value, see types above|
|comment|Optional free form comment field|

## Weights
The weights requirement instructs the driver to capture the outcome from a weighbridge. This is indepent of the Weigh Bridge activity which is meant to capture the outcome of a municipal weigh bridge.

### Requirement

There is no additional configuration for this requirement.

```
{
    "integration_key": "string",
    "label": "string",
    "is_optional": true
}
```

### Outcome

```
{
    "unit": "string",
    "value": "string",
    "integration_key": "string",
    "status": "Success",
    "status_reason": "string"
}
```

|Type|Description|
|----|-----------|
|unit|Represents the unit of measure being used and must be one of `tons` or `metric_tons`|
|value|The numerical value captured at the weightbridge|

## Images

Instructs the driver to capture one or more images with the camera of the phone. The images should be uploaded to blob storage while the image url should be sent back in the outcome.

### Requirement

```
{
    "multiple": true,
    "integration_key": "string",
    "label": "string",
    "is_optional": true
}
```

|Type|Description|
|----|-----------|
|multiple|When `true` the driver should be allowed to capture multiple images for the same outcome|

### Outcome

```
{
    "image_urls": [
        "string"
    ],
    "comment": "string",
    "integration_key": "string",
    "status": "Success",
    "status_reason": "string"
}
```

|Type|Description|
|----|-----------|
|image_urls|One or more images urls representing the blob storage url|
|comment|Optional free form text comment|
