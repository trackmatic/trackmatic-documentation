# Authentication

The Trackmatic API offers three methods of authentication and are described below. Users can use either their email address or identity number as their username.

## Username & Password

By default when a user is created a password request will be sent to the user via email. Once a password has been set a user can use that password to authenticate against the api.

```
POST /account/auth

{
    "username": "string",
    "password": "string"
}
```

## Username & Pin

When a pin has been set a user can use the pin in place of their password. The same api call can be used as per above.

```
POST /account/auth

{
    "username": "string",
    "password": "string"
}
```

## Api Key

For integrations an api key can be created which will allow you to limit access for that integration to only the relevant integration api's. A token can be obtained using an API key as follows:

```
GET /account/auth?apiKeyId=string
```