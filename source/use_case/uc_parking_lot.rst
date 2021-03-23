Outdoor Wireless Example : Parking Lot Surveillance
===================================================

.. image:: /images/uc_parking.png
    :align: center
    :width: 100%

Parking lot surveillance is more important than ever. Whether you need the IP camera for security surveillance, for better curb side service, or simply for car counting or parking alerts with artificial intelligence. You may want to install a camera outside of your building or on the light pole in the parking lot.

Topology
----------------------------------------

Connecting to a camera installed on the light pole of the parking lot is easy. Simply install a Pharos CPE configuring as a client. Powering up the CPE with the PoE injector comes with the CPE product. Connect to the camera with the second port of the PoE injector. 

.. image:: /images/uc_camera_connection.png
    :width: 80%
    :align: center

On the office side, if the signal is strong enough that the CPE can detect the signal, you don’t have to do any change. Otherwise, install another Pharos CPE outside of the building. Again, connecting the CPE to the PoE injector and connecting the other port of the PoE injector to the office network. 

.. note::
	Please reference the `How to calculate the wireless range`_ for requirements of the equipment each way. When doubt, use a pair of the same CPE to build a wireless bridge for the best performance.

.. _How to calculate the wireless range: wireless_range.html

Installation
------------

* Reference `how to set up a CPE`_ for detail instructions on the CPE set up.
* Remember using a shielded Ethernet cable to connect to the access point and ground the PoE injector proper to provide the best lighting protection.

.. _how to set up a CPE: how_to/cpe_onboarding.html
    