***********
Active Load
***********

The active load api call allows a driver to pull the current active load from the system. There can only ever be one active load for any given driver. If there is no current active load the API will return a 404 response indicating that there is no active load found.

Allocation
==========

The allocation describes the various components which have been allocated to the load. The allocation object is important when capturing odometer readings as the odometer configuration is defined for each asset in this section.

Consignments
============

Header information about the consignment is enclosed in this section. It is intended to be used for display purposes only.

Travel Plan
===========

The travel plan describes what the driver has been requested to execute. The travel plan consists of two or more points of interest with activities to be executed at each one. The driver is expected to execute the load according to the sequence that the points of interest and activities appear in the message.

Point of interest
=================

A point of interest represents the physical location which the driver is required to drive to in order to perform their activities. The point of interest contains an address which provides the relevant address information as well as the geofence data representing the physical geofence of the destination. The geofence can be used to test whether the driver has arrived or left a stop.

Planned Path to
===============

The planned path represents the travel path to be taken from the previous stop to the current one and provides information on travel times and distance.

Activities
==========

The activities describe what the driver needs to do when he/she arrives at a stop. A stop is made up of 0 or more activities. The execution sequence contains a list of the activity reference numbers and describes the order in which the activities should be executed. Each activity has 0 or more requiremnts. 

Requirements
============

A requirement defines the workflow and data which shoud be captured for every activity. The workflow for each activity should be built up from this metadata. The execution sequence contains a list of the requirement reference numbers and describes the order in which the requirements should be executed.