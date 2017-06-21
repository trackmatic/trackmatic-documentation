# Drivers Api

## Technical Documentation
For more information on available calls and messages structure [goto the open api docs](http://secure.trackmatic.co.za/documentation/loads-drivers.html)

## Active Load

The active load api call allows a driver to pull the current active load from the system. There can only ever be one active load for any given driver. If there is no current active load the API will return a 404 response indicating that there is no active load found.

### Allocation

The allocation describes the various components which have been allocated to the load. The allocation object is important when capturing odometer readings as the odometer configuration is defined for each asset in this section.

### Consignments

Header information about the consignment is enclosed in this section. It is intended to be used for display purposes only.

### Travel Plan

The travel plan describes what the driver has been requested to execute. The travel plan consists of two or more points of interest with activities to be executed at each one. The driver is expected to execute the load according to the sequence that the points of interest and activities appear in the message.

### Point of interest

A point of interest represents the physical location which the driver is required to drive to in order to perform their activities. The point of interest contains an address which provides the relevant address information as well as the geofence data representing the physical geofence of the destination. The geofence can be used to test whether the driver has arrived or left a stop.

### Planned Path to

The planned path represents the travel path to be taken from the previous stop to the current one and provides information on travel times and distance.


### Activities

The activities describe what the driver needs to do when he/she arrives at a stop. A stop is made up of 0 or more activities. The execution sequence contains a list of the activity reference numbers and describes the order in which the activities should be executed. Each activity has 0 or more requiremnts. 

### Requirements

A requirement defines the workflow and data which shoud be captured for every activity. The workflow for each activity should be built up from this metadata. The execution sequence contains a list of the requirement reference numbers and describes the order in which the requirements should be executed.

## Asset Selection

There are a number of outcomes and activities which require the driver to select the related asset.

The system must support 2 methods of capture, the first must allow the driver to scan a QR Code, the second must allow him to manually search through a list of assets.

The list of assests used for the selection process will come from one of two places. When on an active load the driver must be presented with a list of assets obtained from the allocation section of the load. When not on a load the driver must be presented with a list of pre-fectehd assets from the assets endpoint.

### Asset Validation

The purpose of the asset validation is to ensure that the driver is capturing information for the correct asset.

For requirements or activities which allow for asset selection there are two fields which can be provided which describes the nescessary asset validation. These two fields are `asset_id` and `asset_type`

When `asset_id` has been supplied, the selected asset id must match the provided asset id exactly.

When `asset_type` has been supplied the selected asset must be of the same type.

When an asset is either scanned or manually selected via search, and an asset type has been provided, the above validations must be applied.

If `asset_id` or `asset_type` has not been provided the system should accept what ever the driver selects.

## Money

When a driver is required to capture money for an outcome or an activity, it is possible that they they are dealing with multiple currencies.

A list of available currencies will be provided in these instances. If only one currency is provided that should be automatically selected.

The list of currencies are provided with an id and a symbol. The id is what should be posted back on the ourcome or activity. The symbol must be used to display to the user.

```
  {
    "id": "ZAR",
    "symbol": "R"
  }
```

## Requirements & Outcomes

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

## Session Management

A driver must obtain a session before being able to perform any actions on the api. The session is used to bind the driver, asset and device together so the system knows Which device is being used to track which driver and asset.

### Retrieve an active session

`GET /{organisationId}/sessions` can be used to retrieve an active session. If no active session exists a 404 result will be returned. Your app shoud check for an active session before trying to create a new one.

### Creating a session

The following api call will allow you to create a new session which binds the currently logged in user to the asset and device provided. Any attempt to create a new session with any combination of the below will cause an error to be thrown.

```
POST /{organiastionId}/sessions

{
    "asset_id": "",
    "device_id": ""
}
```

### Revoking a session

If a session was created by mistake or the driver wishes to manually release the session you can do this via the following api call. A reason for revoking the session must be provided.

```
PUT /{organiastionId}/sessions{sessionId}/revoke

{
    "reason": "",
}
```

### Closing a session

A session shoud be closed only once all data has been flushed from the store and forward mechanism. Closing a session before that could result in data loss.

```
PUT /{organiastionId}/sessions{sessionId}/close
```