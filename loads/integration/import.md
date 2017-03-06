# Import

The import API provides a way to upload the complex load structure in a denormalized format. There are many moving parts to a load care needs to be taken when building an integration to ensure a reliable and robust result.

Each message represents a single load along with all of its associated data. Once initial validation has been performed on the message the load is dispatched asynchrnously to be processed by the server. This means that the load may not be available immediately after a 200 response code is received. A web hook can be registered to notify you once the upload is complete.