Outdoor Wireless Example : RV Park
==================================

.. image:: /images/uc_rv.png
    :width: 100%
    :align: center

Traveling with RV is fun, not having the Internet connection is not. Providing a good WiFi connection to the RV campers is import and necessary. But, how?

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


What about the line-of-sight requirement?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

It is critical in point-to-point CPE communication and has alternatives in EAP mesh networking. Any non-direct wireless beam from the sender to the receiver will be considered interference. Especially in miles long communications. However, it is more tolerated in shorter outdoor wireless communications. The EAP mesh networking not only can pick up the direct  wireless beam, but also can take reflected and deflected beams as the wireless path. The wireless MIMO coordinates the direct and indirect communications. So, the wireless communication is still available with partial blocking by the woods or leaves.

On the RV
---------

You may visit different campgrounds from time to time and the WiFi signal quality will be varied from one to another. A sensitive wireless antenna (receiver) is what you need to receive the best signal from the campground office.

.. image:: /images/uc_rv_park_cpe.png
    :width: 60%
    :align: center
    
The Pharos CPE has 2.4GHz (CPE210) and 5GHz (CPE510). Most of the campgrounds provide 2.4GHz service. Therefore, the CPE210 is your best bet as a receiving device. 5GHz has less interference, you may get better traffic over 5GHz if the campground provide the service.

.. image:: /images/uc_rv_park_cpe_topo.png
    :width: 80%
    :align: center  
    
Installation
------------

* Reference `Omada SDN Cookbook`_ for detail instructions of EAP mesh network set up.
* Reference `how to set up a CPE as a receiver`_ for detail instructions RV receiver set up.
* Remember using a shielded Ethernet cable to connect to the access point and ground the PoE injector proper to provide the best lighting protection.

.. _Omada SDN Cookbook: https://omada-sdn.readthedocs.io/en/latest/index.html

.. _how to set up a CPE as a receiver: how_to/cpe_onboarding.html#set-up-cpe-as-an-client