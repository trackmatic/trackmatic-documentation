*******
Drivers
*******

Session Management
==================

A driver must obtain a session before being able to perform any actions on the api. The session is used to bind the driver, asset and device together so the system knows Which device is being used to track which driver and asset.

Retrieve an active session
--------------------------

:code:`GET /{organisationId}/sessions` can be used to retrieve an active session. If no active session exists a 404 result will be returned. Your app shoud check for an active session before trying to create a new one.

Creating a session
------------------

The following api call will allow you to create a new session which binds the currently logged in user to the asset and device provided. Any attempt to create a new session with any combination of the below will cause an error to be thrown.

.. code-block:: C#

 POST /{organiastionId}/sessions

 {
    "asset_id": "",
    "device_id": ""
 }


Revoking a session
------------------

If a session was created by mistake or the driver wishes to manually release the session you can do this via the following api call. A reason for revoking the session must be provided.


.. code-block:: C#

 PUT /{organiastionId}/sessions{sessionId}/revoke

 {
    "reason": "",
 }



Closing a session
-----------------
A session shoud be closed only once all data has been flushed from the store and forward mechanism. Closing a session before that could result in data loss.

:code:`PUT /{organiastionId}/sessions{sessionId}/close`

Active Load
===========

The active load api call allows a driver to pull the current active load from the system. There can only ever be one active load for any given driver. If there is no current active load the API will return a 404 response indicating that there is no active load found.

Allocation
----------

The allocation describes the various components which have been allocated to the load. The allocation object is important when capturing odometer readings as the odometer configuration is defined for each asset in this section.

Consignments
------------

Header information about the consignment is enclosed in this section. It is intended to be used for display purposes only.

Travel Plan
-----------

The travel plan describes what the driver has been requested to execute. The travel plan consists of two or more points of interest with activities to be executed at each one. The driver is expected to execute the load according to the sequence that the points of interest and activities appear in the message.

Point of interest
-----------------

A point of interest represents the physical location which the driver is required to drive to in order to perform their activities. The point of interest contains an address which provides the relevant address information as well as the geofence data representing the physical geofence of the destination. The geofence can be used to test whether the driver has arrived or left a stop.


Planned Path to
---------------

The planned path represents the travel path to be taken from the previous stop to the current one and provides information on travel times and distance.


Activities
----------

The activities describe what the driver needs to do when he/she arrives at a stop. A stop is made up of 0 or more activities. The execution sequence contains a list of the activity reference numbers and describes the order in which the activities should be executed. Each activity has 0 or more requiremnts. 

Requirements
------------

A requirement defines the workflow and data which shoud be captured for every activity. The workflow for each activity should be built up from this metadata. The execution sequence contains a list of the requirement reference numbers and describes the order in which the requirements should be executed.