.. TP-Link USA Outdoor Solution Guide master file

TP-Link USA Outdoor Solution Guide
==================================

There are many TP-Link products can extend the Internet coverage at your home and beyond. This document intended to discuss the various ways to extend your home network to your backyard, or remote barn house.

Near Site or Remote Site
------------------------

We will discuss the different solution to extend the Internet around your house within 100 meters (300 feet) or farther connection more than 300 feet and less than 18 miles to your other personal property. You do have more choices to extend the home network just around your house. To extend the Internet to the remote house or second work place, you need to build a point-to-point wireless bridge and then re-broadcast the signal on remote location. Different connectivities has different environmental requirements. Please review your situation and then choose the best one.

Near Site network extension (up to 100 meter or 300 feet)
---------------------------------------------------------

You probably have very good indoor wireless, and you want to extend the signal to the patio or your backyard. The wireless signal can easily penetrate through the window glass, but it is hard to penetrate the stucco wall. Most of the stucco walls installed the mesh wire to hold the material. The mesh metal is the perfect blocker of the wireless signal. It can prevent the wireless interference from outside of the house. At the same time, it can prevent the signal transmit from indoor to the outdoor as well.

You need to set up a wired communication to penetrate the exterior building wall. You can choose power line communication technology or simply the traditional network cable.

.. image:: /images/mesh_wires.jpeg
    :width: 50%
    :align: center

Power line communication
~~~~~~~~~~~~~~~~~~~~~~~~

If you want to extend the wireless signal from indoor to outdoor patio. The TL-WPAxx series product is the choice. It comes with two power line communication adapters. One can relay the data from the network cable to the power line and the other adapter has additional capability to broadcast the WiFi signal to your computer or phone directly.

.. image:: /images/PLC-patio.png
    :width: 60%
    :align: center

Plug-in the first PLC adapter on one of the power sockets in the house. Connect the network port on the PLC adapter to the home router with network cable. Plug the second PLC adapter (with wireless feature) on the socket on your patio.

.. note:: 
   Both PLC adapters are rated as indoor devices. If there is a change that the PLC adapter on the patio will be splashed by water, please provide appropriate protection to the PLC adapter.

PLC for the backyard office
^^^^^^^^^^^^^^^^^^^^^^^^^^^

If you build your backyard office or summer house lately, you probably bury a power line from the main house to the isolated shed. If you do have a power line to the shed and no data wire, there is another chance to extend your network easily using the buried power line.

.. image:: /images/PLC-backyard_office.png

Using the power line for the backyard office, you need to find the direct connect electric loop connecting your home and the backyard office. In most installations, the power line is connected between two circuit breaker panels. One on the main house and one on the backyard office. Therefore, The PLC adapters have to communicate to each other through at least 2 circuit breakers. Circuit breakers can be a challenge to the power line communication, with the latest technology the signal can still pass through them, but not the AFCI or GFCI type circuit breakers. Find the close by power socket to the power panel to build the best communication that you can have.


.. image:: /images/AFCI_Breaker.png
    :width: 10%
    :align: center

.. note:: 
   Other than AFCI or GFCI circuit breaker, you need to avoid the surge protector, power strip, and UPS. Those devices will filter the high frequency transpassing which the power line communication depends on.

Outdoor Wireless Access Point
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If your patio is not shedded or the power line communication was not the best choice. You can choose to install an outdoor access point.
 
There are 2 different choices of the outdoor wireless access points from TP-Link, the omni-directional EAP outdoor access points (EAP225-Outdoor and EAP110-Outdoor), and the directional CPE outdoor access points (CPE210, CPE510, and CPE710). All outdoor wireless access points come with waterproof housing which can be exposed with cover or not.

Omni-directional EAP Outdoor Wireless Access points
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
The EAP Outdoor wireless access points are part of Omada SDN business network. You can control the indoor and outdoor network with the same Omada SDN controller. Or, you can use the Omada outdoor EAP as a standalone wireless access point without a controller. Two of the models are available:
 
* `EAP110-Outdoor 2.4GHz N300 Outdoor Wireless Access Point`_ |ExtLink|
* `EAP225-Outdoor dual-band AC1200 Outdoor Wireless Access Point`_ |ExtLink|

.. _EAP110-Outdoor 2.4GHz N300 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/ceiling-mount-access-point/eap110-outdoor/

.. _EAP225-Outdoor dual-band AC1200 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/ceiling-mount-access-point/eap225-outdoor/

.. note:: 
   There are more features available with the EAP working in controller mode. If you do have a good indoor EAP wireless signal right outside of the house, it is possible to establish a wireless mesh network from inside your house to outdoor area. For more information, please reference to the `Omada SDN Set Up Guide`_ |ExtLink|.

.. _Omada SDN Set Up Guide: https://omada-sdn.readthedocs.io/en/latest/

.. image:: /images/eap225-patio.png
    :width: 80%
    :align: center

Set up the EAP Outdoor wireless access point is easy. There is a PoE injector that comes with the package. Plug one end of the network cable to the Outdoor EAP and plug in to the **PoE** port on the PoE injector with the other end of the network cable. Prepare another network cable connecting the network port of the PoE injector to your home gateway.

.. note:: 
   check up this `how to guide`_ |ExtLink| for detailed steps setting up the EAP in standalone mode.

.. _how to guide: https://omada-sdn.readthedocs.io/en/latest/

The coverage of the wireless can be 100 meter (300 feet) radius from the access point.

.. image:: /images/EAP225-coverage.png
    :width: 80%
    :align: center

Outdoor wireless mesh networking
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Extending radio signal with outdoor EAP is different to the outdoor CPE. The only outdoor EAP supports wireless extender feature is the EAP225-Outdoor. To extend the radio signal, you have to set up a wireless mesh network. The wireless mesh network requires a controller to coordinate the traffic, so a basic topology of outdoor EAP mesh network can be like this.

.. image:: /images/eap225-mesh.png
    :width: 80%
    :align: center

The EAP225-Outdoor mesh can wirelessly link back to the network up to 3 hops. A complex yacht club wireless deployment can be achieved easily with the outdoor EAP mesh network.

.. figure:: /images/eap225-yacht.png
    :width: 80%
    :align: center
    
    A yacht club wireless deployment example with EAP225-Outdoor


Directional Outdoor Wireless Access points
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
The CPE Outdoor wireless access points are part of Pharos long distance wireless bridge products. You can also use it to extend the signal around your house if the coverage is good to you:
 
* `CPE210 2.4GHz N300 Outdoor Wireless Access Point`_ |ExtLink|
* `CPE510 5GHz N300 Outdoor Wireless Access Point`_ |ExtLink|
* `CPE710 5GHz AC867 Outdoor Wireless Access Point`_ |ExtLink|

.. |ExtLink| image:: /images/External_Link.png
                     :width: 10 px

.. _CPE210 2.4GHz N300 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/outdoor-radio/cpe210/

.. _CPE510 5GHz N300 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/outdoor-radio/cpe510/

.. _CPE710 5GHz AC867 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/outdoor-radio/cpe710/

The CPE Outdoor wireless access point provides a strong outgoing signal as well as a high  receiving sensitivity. It can extend the range of the wireless and the communication range will be decided by the lower powered transceiver. Most of the time, it is your laptop or cell phone if you don’t use a pair of CPE.

.. note::
   Here’s a reference page about `how to calculate the wireless range`_ 

.. _how to calculate the wireless range: wireless_range.html

Different model of the Outdoor CPE has different beam width 

.. table:: Access point radio beamwidth
    :align: center

    +-----------+--------+--------+--------+--------------------+
    | Model     | CPE210 | CPE510 | CPE710 | CPE710 - Feed only |
    +===========+========+========+========+====================+
    | Beamwidth | 65°    | 45°    | 9°     | ~ 45°              |
    +-----------+--------+--------+--------+--------------------+
    | Antenna   | 9 dBi  | 13 dBi | 23 dB  | ~                  |
    +-----------+--------+--------+--------+--------------------+

Choose the Outdoor CPE which has a good coverage and the best wireless gain for the best result.

.. image:: /images/cpe_coverage.png
    :width: 80%
    :align: center

One of the way using the CPE710 is use the access point with the feed antenna only, without reflective dish. The reflective dish can refocus the wireless signal to a certain direction with concentrated power. If you use the CPE710 in near site, just around your house, it is possible not using the reflective dish.

.. image:: /images/cpe710-feed-mode.png
    :width: 80%
    :align: center

Remote Site network expansion (more than 100 meter or 300 feet and up to 18 miles)
----------------------------------------------------------------------------------

If you have a barn house, a remote surveillance camera, or a video doorbell on the vineyard entrance, and the distance from your house is more than 300 feet, you can use the outdoor CPE building a wireless bridge to expand the network.

On the remote site, you can broadcast the wireless signal with an additional wireless access point when necessary.

.. image:: /images/cpe-dock_house.png
    :width: 80%
    :align: center

.. toctree::
   :maxdepth: 2
   :caption: Document Index:

   wireless_range
