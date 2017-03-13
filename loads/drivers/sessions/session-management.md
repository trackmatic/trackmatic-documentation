# Session Management

A driver must obtain a session before being able to perform any actions on the api. The session is used to bind the driver, asset and device together so the system knows Which device is being used to track which driver and asset.

## Retrieve an active session

`GET /{organisationId}/sessions` can be used to retrieve an active session. If no active session exists a 404 result will be returned. Your app shoud check for an active session before trying to create a new one.

## Creating a session

The following api call will allow you to create a new session which binds the currently logged in user to the asset and device provided. Any attempt to create a new session with any combination of the below will cause an error to be thrown.

```
POST /{organiastionId}/sessions

{
    "asset_id": "",
    "device_id": ""
}
```

## Revoking a session

If a session was created by mistake or the driver wishes to manually release the session you can do this via the following api call. A reason for revoking the session must be provided.

```
PUT /{organiastionId}/sessions{sessionId}/revoke

{
    "reason": "",
}
```

## Closing a session

Sessions are closed automatically by the system as a result of some other action such as closing a route. The driver does not have the ability to explicitly close a session.