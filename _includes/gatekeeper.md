## Overview

The pupose of Gatekeeper is to record movements with a purpose in and out of facilities via predefined Gates, and to provide additional instructions to drivers entering the facility for a specific purpose.
The Gatekeeper module was developed to function as a standalone module or to integrate with other modules like Link-Facilities where bookings are scheduled. 

## Facility

Defines the location/area of the organisation being visited.

## Gate

Point of entry or exit out of the facility. A gate can be setup to allow **Movements** of eith type: `InBound`, `OutBound` or both.

## Visit

A visit groups Movements together at the facility along with a `Purpose`, recorded `Checkpoints` and other auditing information.

### Visit Types

- Booking: Booking scheduled on the Link-Facilities module.  A gate-pass is issued which facilitates the entry process at the gate by identifying the purpose, and optionally providing instructions for the driver to get to the Bay.
- Visitor: Visitors at the facility.
- Ctc: Customer To Collect
- Utility: Utility run performed consisting of an exit and entry on return.

### Visit Statusses

- Pending
- Active
- Completed
- Cancelled

## Checkpoint

Each entry/exit is recorded as a checkpoint on the `Visit` where various device scans and/or fields of information are captured. Once the final checkpoint is captured, the Visit is `Completed`.

## (Checkpoint) Configuration

Checkpoint configurations can be configured for combinations of `Facility /MovementType / VisitType` which includes Fields to be captured/scanned.

### Checkpoint Fields

These are the fields that need to be recorded at `Checkpoints`. Fields can be marked as `optional` and `validation` can be enabled to perform validation checks on the values recorded.

### Checkpoint Field Types

- asset_license:            Scanned asset license disc (encoded)
- vehicle_registration_no:  Captured vehicle registration number
- vehicle_odometer:         Captured vehicle odometer reading
- ctc_documentcapture:      Customer to collect document barcode
- trailer_registration:     Captured trailer registration number
- linkfacilities_bookingid: Booking Id
- driver_id:                Captured driver identity number
- driver_licenseno:         Captured driver license number
- driver_license:           Scanned driver license (encoded)
- driver_contact:           Captured driver contact number
- crew_id:
- crew_contact:             Captured crew member contact number
- load_id:
- load_contact:
- person_id:
- person_name:              Captured person name
- person_contact:           Captured person contact number
- temperature:              Captured temperature reading

## Operator

Operators are created the same way as in other modules, granting access to the Gatekeeper mobile application.

## Device

A mobile device that is `registered` against one or more gates. See api [here](https://trackmatic.github.io/trackmatic-documentation/rest/gatekeeper/open-api#operation/AppGates_Register).
