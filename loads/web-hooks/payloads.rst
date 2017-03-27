****************
Webhook Payloads
****************

Load Activated :code:`load.activated`
=====================================
.. code-block:: C#

    {
        "when": "2017-03-23T08:32:10.069287Z",
        "where": [ 0, 0 ],
        "load_id": "string",
        "reference": "string",
        "requested_date": "2017-03-23T08:30:50.2078258Z",
        "allocation": {
        "driver": {
            "id": "string",
            "name": "string",
            "reference": "string"
        },
        "vehicle": {
            "id": "string",
            "reference": "string",
            "registration": "string",
            "fleet_number": "string"
        },
        "assets": [],
        "accessories": {
            "pallet_jack": null,
            "load_lock_rails": 0,
            "fuel_card": null
        }
    }

Pickup Started :code:`load.pickup.started`
====================================

.. code-block:: C#


Pickup Completed :code:`load.pickup.completed`
========================================

.. code-block:: C#


Dropoff Started :code:`load.dropoff.started`
======================================

.. code-block:: C#


Dropoff Completed :code:`load.dropoff.completed`
==========================================

.. code-block:: C#
