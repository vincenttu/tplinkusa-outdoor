Outdoor Wireless Example : RV Park
==================================

Traveling with RV is fun, not having the Internet connection is not. Providing a good WiFi signal to the whole RV campground is necessary today. But, how?

Single AP coverage 
------------------

In a small size of the campground, a single access point can service all the campers. The EAP225-Outdoor has recommended coverage 100 meters (300 feet) with the maximum coverage 200 meter radius. The dual band access point provides services on both 2.4GHz and 5GHz. MU-MIMO makes the multiple user access more efficient.

.. image:: /images/uc_rv_park_1.png
    :width: 80%
    :align: center

Outdoor wireless mesh
---------------------

A large size of the RV park may need more outdoor access point for the coverage. This is an example of 14 acre RV park WiFi. It was planned using four (4) EAP225-Outdoor for the overall coverage. The EAP225-Outdoor is capable of creating the back link to the root access point wirelessly. No cabling is required. It supports up to three (3) uplink hops. 

.. image:: /images/uc_rv_park_mesh.png
    :width: 80%
    :align: center

The outdoor mesh network can be controlled by an OC200 network controller. The controller monitors the network all the time. It creates, maintains, and heals the wireless mesh network.

.. image:: /images/uc_rv_park_mesh_topo.png
    :width: 80%
    :align: center

    
Installation
------------

* Reference `Omada SDN Cookbook`_ for detail instructions on access point set up.
* Remember using a shielded Ethernet cable to connect to the access point and ground the PoE injector proper to provide the best lighting protection.

.. _Omada SDN Cookbook: https://omada-sdn.readthedocs.io/en/latest/index.html