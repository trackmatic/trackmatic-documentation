# Loads Api

## Loads in Context
The loads module is made up of a number of interconnected components which will be described in this section.

### Entity

An Entity represents an organisation, business, customer or individual which you interact with within the context of the loads module.

Entities do not mean a whole lot on their own and are primarily used as a building block for consignments and loads. When creating consignments or loads you will be able to select from a pre-captured list of entities preventing you from having to capture the entity information from scratch.

The necessary tools are provided to assist you in managing entities by searching them, creating new ones, editing existing ones and deleting unused ones.

### Shipping Address

A shipping address represents the business address of your entities. The relationship between entities and shipping addresses is many to many giving you the flexibility to model your organisations entity to shipping address relationships.

Much like an entity the shipping address is a convenience feature preventing you from having to capture this information over and over again when creating consignments and loads.

### Location

A location represents the physical location of a shipping address marked out on the planet. A location has a shape, namely radius or polygon, which is one or more geographical points marked out on a geo spatial map.

The location is attached to a loads stop and used to detect when an asset enters or leaves the demarcated area.

A shipping address is linked to the shipping address as a convenience feature so that when you are creating loads you do not need to recapture the location information.

When a load is a created the system will look at the entities associated shipping addresses and pull out the location information when a stop is created on a load.

The concept of a location is an important technical aspect of the Trackmatic system in general. It is the mechanism used to track assets in context. In the Tracking module we have the concept of locations. We have purposefully changed the name from location to location in the the Loads module in order draw a distinction between them.

While a location can be backed by a Location in the Tracking module it does not have to be. When it is not backed by an underlying Location it is considered by the loads module as ad-hoc.

In the context of the Tracking module the Location is used to track an asset moving in and out of the pre-defined location, while in the loads module it simply used as a template to facilitate the creation of stops.

### Asset

An asset represents the physical assets which you need to track. An asset is associated with a type namely vehicles, trailers or forklifts.

The assets themselves are managed via the Fleet module. When creating a load you will be require to associated that load with one or more assets. For this reason the loads api has a read only view of the assets loaded up from the fleet module.

### Operator

Operators represent the people responsible for executing the load. Like assets they are managed by the fleet module however a read only view of them has been provided via the loads api for your convenience.

Operators must have one or more types namely driver or crew. In the context of a mobile app the operator executing must also be a user so that they have a username and pin granting them access to the system.

Both the user and the operator are backed by a person in the Trackmatic ecosystem. People are managed via the Organisations module and provides a single identity for all the roles that a person may fulfill within the system. Details on the user is outside the scope of this article however you can find out more about this under the [Organisations]({{'/rest/organisations' | prepend: site.github.url}}) module documentation.

### Consignment
The official definition of a consignment is as follows:

> Consignment is the act of consigning, the act of giving over to another person or agent's charge, custody or care any material or goods but retaining legal ownership until the material or goods are sold. That may be done for the purpose of shipping the goods - [Wikipedia](https://en.wikipedia.org/wiki/Consignment)

In the loads module a consignment represents the business information describing goods which need to be shipped.

A consignment must be allocated a Consignee and Consignor where each of these can be, but do not have to be, selected from a pre-loaded entity described above. When an entity is not selected and the consignor and consignee are set manually they are considered to be ad-hoc entities by the loads module.

A consignment must be allocated one or more pickups or drop offs. A pickup described where the goods need to be picked up form, while the drop off describes where the goods need to be dropped off at. The pickup and drop off are both activities which will be described in more detail later in this document.

When a consignment is allocated to a load the pickup and drop offs are assigned to one or more stops on load. The stop is built up from the shipping address and location information extracted for the consignments pickups, drop offs and associated entities.

A consignment passes through a number of statuses in its life cycle:

|Status|Description|
|---|---|
|Draft|When a consignment has been created but not yet made available for allocation to a load. Changes can only be made to a consignment while in draft status|
|Un-allocated|When a consignment is complete and available to be planned onto a load|
|Allocated|When a consignment has been allocated to a load|

### Activity

An activity serves as instructions to the operator on what work to performed at a specified point during the load.

Activities can be either planned or un-planned. When planned they will be associated with a load at a specific stop. When a driver reaches they stop they will be requested to perform the associated activities. When unplanned the operator will have the ability to select an activity to perform.

There are many types of activities available in the loads module:

- Pickups
- Dropoffs
- Odometer readings
- Rest stops
- Fatigue assessments
- Border crossings
- Weighbridges
- Fuel stops
- Pallet drops
- Breakdown

While most activities can be both planned and un-planned there are a few exceptions which prevent them from being used in both contexts.

Pickups and Drop offs for instance require a certain amount of planning with the context of loads and therefore need to be planned before hand.

A breakdown for instance will hopefully never be planned and therefore may not be added to a load as a planned activity.

#### Requirements & Outcomes

Each activity can describe one or more requirements which need to be fulfilled as part of the execution of an activity.

When the operator executes an activity they will be requested to capture information describe to them by the requirement. The information which has been captured and sent back to the loads api is called on outcome.

The intention of requirements is to provide a way for you to customise the workflow of an activity. Each activity provides a success and failure flow allowing you to specify different requirements depending on whether the activity was executed successfully or not.

Currently the system support the following activities:

- Signatures
- Cash on delivery
- Document scans
- Image capture
- Odometer readings
- Pallet transfers
- Pallet drops
- Service ratings
- Proof of deliveries
- Weighbridge readings
- E-Documents

### Load
The load is the most important and complex component of the loads module. The load is where the rubber hits the road in the literal sense.

A load serves as a set of instructions to the driver (type of operator) on how to execute a given load.

A load consists of a collection of consignments and activities arranged within stop.

#### Stops
The stop represents a specific place on the planet (Location) which the driver needs to drive to in order to perform their pre-defined work (Activities). When they arrive at a stop they will be required to interact with various people (Entities) to get their work done.

It should be clear that a stop can only exist within the context of a load and is the component which bring Entities, Shipping Addresses, Locations and Activities together to form the travel plan.

The stops are connected by a path. The path represents the physical path which should be followed in order to get to the stop. The path is used by the navigation system to direct to the operator to the stop. The path has a time and distance component which is used to measure the operators progress while moving between stops.

#### Travel Plan
The travel plan consists of two or more stop and describes the sequence in which the stop should be visited.

#### Allocation
The load allocation represents the components which have been allocated to facilitate the execution of the load. The allocation exists primarily of an operator and a vehicle (the asset assigned to haul the load). Supporting assets can also be allocated to a load to facilitate the management of those assets.

An operator can only ever have one active load at a time however multiple loads can be allocated to a single operator in a planned status. A load can be transferred between assets and operators if necessary.

#### Status
A load goes through a number of statuses within its life cycle:

|Status|Description|
|---|---|
|Planning|When a load is in the process of being planned it is in the planning status|
|Planned|When a load is ready for execution it is in the planned status|
|Executing|When an operator activates a load it goes into the executing status|
|Closed|When a driver has completed a load and all tracking and activity data has been captured it goes into the closed status|
|Cancelled|A planned load can be cancelled which means that it is never intended to be executed|

#### Promptitude

Promptitude is used to describe if the driver was early, late or very late for a given stop or activity. The thresholds to determine the promptitude are configureable at the organisation level.


## Supporting Apis

|API Name|Description|   |
|--------|-----------|---|
|Drivers|Drivers api|[read more](./drivers/index.md)|
|Integration|Integration api|[read more](./integration/index.md)|
|Shippers|Shippers api|[read more](./shippers/index.md)|