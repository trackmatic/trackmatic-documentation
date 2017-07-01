# Welcome

Welcome to the Trackmatic technical guide. This guide will take you through various business and technical concepts which you will need to successfully integrate to the Trackmatic backend systems.

## Modules

The Trackmatic ecosystem is divided into a number of modules. Each module provides functionality for a specific use case of the Trackmatic system. The remainder of this section will provide a high level over of each module.

### [Organisations](/rest/organisations)

The purpose of the organisation module is to allow users to manage master data and access control to the other modules of the system.

When working with the various Trackmatic apis the first thing you will need to know is which organisation you are working with. The organisation represents a tenant of the trackmatic system. Accessing an organisation requires an [access token](/rest) for that organisation.


### [Fleet](/rest/fleet)

The fleet module provides users with the ability to perform various fleet management tasks. The are two fundamental components of the fleet module which are used by other modules of the system:

- Assets - An asset represents the physical asset managed by a fleet manager. An asset can be a vehicle, trailer or forklift.
- Operators - An operator is a person who operates an asset. An operator can be either a driver, crew member or both.

### [Tracking](/rest/tracking)

The tracking module provides visibility into the movement of the fleet. This is done using real time dashboards which represent the geospatial position of an asset on a map in relation to predefined locations and zones.

### [Loads](/rest/loads)

The loads module provides the nescessary functionality to manage primary distribution concerns. At a high level it deals with planning, dispatch, execution and debriefing of loads.