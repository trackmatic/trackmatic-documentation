---
layout: default
title:  "Username Changes"
date:   2018-05-09 09:42:00 +0200
categories: accounts
excerpt: Important username changes
---

# Username Changes

Some changes have been made to how usernames are created in the system in order to clear up confusion as well as allow operators to have a single username and password for multiple organisations.

Previously there was no explicit username field in the system. The system was using either the email and/or identity number as the username and ensuring that those values, when provided, were globally unique across the entire user base.

It is important that the username is globally unique across all users to ensure that we can reliably determine what the user/operator has access to by only providing a username. If this were not the case then the user would need to tell the system which organisation they were trying to log into which is not practical for our use case.

## Explicit Username Field

To avoid confusion an explicit username field as been added. When registering as a user or creating an operator a unique username must be provided.

### Users

When a user is created, either by way of invitation or by creating a new user from the organisation console, a set password will email be sent to the user if they do not already have a password.

At this point the system will check if they have a username assigned. If they do not the system will require them to provide a unique username before being able to set a password.

This flow will allow the user to select their own username and is intended to prevent friction as much as possible when creating a new user.

A user will have the ability to change their username when editing their account information once logged into the system.

The "Forgot Username" functionality will be built into the system once the initial change has been released.

### Operators

Since operators do not have access to the web portal the flow will need to be different when creating an operator.

When assigning a pin to an operator the system will check if a username has been provided. If there is already a username then no additional action will be required other than setting the necessary permissions as is done today.

If a username has not been created it will be up to the user creating the operator to assign a username. Since the username can be anything as long as it is unique the user can choose to provide an email address, identity number or any other suitable value.

At the time of writing there is no way to change an operators username. This feature will be added once the initial change has been rolled out.

## Warning for existing users

In the event that you have been added into the system as both a user and an operator your username will be you identity number. If you have problems signing in after the change takes effect please attempt to log in with both your identity number and email address.

The reason this has happened is that by convention operators used identity numbers and users used email addresses. We have opted to favour the operator username to reduce friction for the mobile users.