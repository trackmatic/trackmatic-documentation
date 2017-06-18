# Webhooks Api

The webhooks api allows you to subscribe to events which occur within the various modules of the Trackmatic system. An Http POST is performed against the provided URI when an event occurs which matches your provided subscription details.

## Subscriptions

A subscription lets you tell Trackmatic which Http endpoint to call when one or more event types are matched. A subscrition takes the following form

```
{
  "name": "string",
  "uri": "string",
  "is_active": true,
  "events": [
    "string"
  ],
  "basic_authentication": {
    ...
  },
  "access_token_authentication": {
    ...
  }
}
```

When an event is raised within Trackmatic a callback is dispatched which will attempt to perform a POST against the URI provided in the subscription.

You can create a single subscription which can match on one or more event types. In this configuration you can make use of the http headers in the request to correctly route and interpret the payload. Alternatively you can configure a subscription per event type.

Subscriptions can be managed from the subscriptions api as per below

```
api/v2/webhooks/subscriptions
```

## Payload format

The format of the payload is specific to each event type. Http headers are appended to each request in order to assist you in determining how to interpret the payload. The following http headers are appended to each request:

|Header Name|Description|Mandatory|
|-----------|-----------|---|
|x-tm-event-name|The name of the event which triggered the callback|yes|
|x-tm-correlation-id|A correlation id may be supplied which can correlate one or more events together|no|
|x-tm-site-id|When an event is site specific the site id will be provided|no|
|x-tm-organisation-id|Indicates which organisation the event was raised on|yes|
|x-tm-aggregate-id|The id of the entity which raised the event. The entity type can be inffered from the event name|yes|

## Failures and Retries

The webhook system is designed to be fault tolerant with at least one delivery of a given payload. Depending on the failure condition it is possible a a message to be delivered more than once and you application will need to deal with this eventuality.

The retry mechnism works as follows:

1. If a callback fails it will be attempted up to 5 times with no delay between messages
2. If the callback is still failing after the above 5 attempts the message will be delayed for 15 minutes before the next retry attempt
3. If the callback continues to fail it will retry with a delay increasing in 15 minute increments up to a maximum of 20 times
4. The message will be retried in this fashion for roughly 24 hours. If the callback is still failing after this period it will be marked as failed in our system and retry attempts will stop
5. Failed messages can be retrieved via the /logs endpoint for any given subscription should you require to manually replay the message.

## Logging & Debugging

All callbacks and dispatch attempts are logged and can be retrieved via `api/v2/webhooks/{organisation_id}/subscriptions/{subscriptionId}/logs?take=128&skip=0`

The logs are useful for determining if an event was raised for a given subscription, what the payload being sent was and what the response from your system was.

The response from the logging endpoint is intentionally unstructured since the request and payload information can be different depending on the event type.

## Security & Authentication

It is considered best practice to use Https transport on your webhook receiving endpoint however http is currently supported.

Authentication can be achieved using IP restrictions or implementing an api key style authentication where the token can be embedded in the url. Where this is not possible we do support 2 simple authentication mechanisms.

### Basic Http Authentication

Basic http authentication can be used by configuring a username and password on your subscription

```
{
  ...

  "basic_authentication": {
    "username": "bob",
    "password": "secret"
  }
}
```

### Access Token Authentication

Access token authentication can be used to define an endpoint which needs to be called first in order to obtain an access token to be used on the web hook request.

The access token configuration allows you to specify a uri where an access token can be retrived, along with the name of the http header where the retrieved token will be attached for subsequent requests.

The respsonse from your access token endpoint must place the access token in the header with the specified header name. The webhook system will extract the header from the response and append it to the subsequent webhook request.

```
{
  ...

  "access_token_authentication": {
    "uri": "http://accesstokens.com?key=secret",
    "header": "Authorization"
  }
}
```