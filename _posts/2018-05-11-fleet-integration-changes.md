---
layout: default
title:  "Fleet Integration Changes"
date:   2018-05-11 11:00:00 +0200
categories: fleet
excerpt: Changes to the fleet integration api
---

# Fleet Integration Changes

We have provided a way for the integration to specify the sites which the assets or operators should belong to. This is intended to make the initial setup of the assets and operators easier for the users.

## Operators

A new field named `site_ids` has been added where you would provide the site ids which you want the operator to belong to. The site id would be created within Trackmatic.

If this field is not provided the operator will be allocated to all sites for the organisation when the operator is created.

If the field is left out for an existing operator then the system will not update the list of sites on the operator.

```
{
  "integration_key": "string",
  ...

  "site_ids": [
    "{site}"
  ]
}
```

## Assets

A new field named `site_ids` has been added where you would provide the site ids which you want the asset to belong to. The site id would be created within Trackmatic.

If this field is not provided the asset will be allocated to all sites for the organisation when the asset is created.

If the field is left out for an existing asset then the system will not update the list of sites on the asset.

```
{
  "integration_key": "string",
  ...

  "site_ids": [
    "{site}"
  ]
}
```