.. TP-Link USA Outdoor Solution Guide master file

TP-Link USA Outdoor Solution Guide
==================================

There are many TP-Link products that can extend the Internet coverage from your home or business to the outdoor area. This document intended to introduce the various ways to extend your indoor network to the outdoor areas, your backyard, remote barn house, yacht club, or campgrounds.

Near site or remote site
------------------------

We will discuss the different solutions to extend the Internet around your house within 100 meters (300 feet) or farther connections. There are more possible solutions to extend the network just around the house. To extend the network to the remote house or second workplace farther than 300 feet, you need to build a point-to-point wireless bridge and then re-broadcast the signal on the remote location. Different solutions have different environmental requirements. Review the different conditions and then choose the best one for you.

Near site network extension (up to 100 meter or 300 feet)
---------------------------------------------------------

You probably have very good indoor wireless, and you want to extend the network to the patio or the backyard. The wireless signal can easily penetrate through the window glass, but it is hard to penetrate the stucco wall. The reason is that most of the stucco walls are installed with the mesh metal wire to hold the filler. The mesh metal wires are the perfect blocker of the wireless signal. It can prevent the wireless interference from outside of the building to protect your home. At the same time, it can prevent the signal transmit from indoor to the outdoor as well.

You need to set up a wired communication to penetrate the exterior wall of the building. You can choose the power line communication technology or simply the traditional network cable.


.. image:: /images/mesh_wires.jpeg
    :width: 50%
    :align: center

Power line communication
~~~~~~~~~~~~~~~~~~~~~~~~

If you have a covered patio or waterproof electric box, you can extend the network with the power line adapters. The TL-WPAxx series power line wireless adapter kit is the easier to apply solution. The power line wireless adapter kit comes with two power line communication adapters. One adapter installed in the indoor can relay the data from the network cable to the power line and the other adapter has additional capability to broadcast the WiFi signal to your computer or phone.

.. image:: /images/PLC-patio.png
    :width: 60%
    :align: center

Plug-in the first PLC adapter on one of the power sockets in the house. Connect the network port on the PLC adapter to the home router with network cable. Plug the second PLC adapter (with wireless feature) on the power socket on your patio.

.. note:: 
   Both PLC adapters are rated as indoor devices. If there is a change that the PLC adapter on the patio will be splashed by water, please provide appropriate protection to the PLC adapter.

PLC for the backyard office
^^^^^^^^^^^^^^^^^^^^^^^^^^^

If you build your backyard office or summer house lately, you probably bury a power line from the main house to the isolated shed. If you do have a power line to the shed and no data wire, you can extend your network easily using the buried power line.

.. image:: /images/PLC-backyard_office.png

Using the power line for the backyard office, you need to find the direct connect electric loop connecting your home and the backyard office. In most installations, the power line is connected between two circuit breaker panels. One on the main house and one on the backyard office. Therefore, The PLC adapters have to communicate to each other through at least 2 circuit breakers. Circuit breakers can be a challenge to the power line communication, with the latest technology the data communication can pass through a simple breaker, but not the AFCI or GFCI type circuit breakers. Find the close by power socket to the power panel to build the best communication that you can have.


.. image:: /images/AFCI_Breaker.png
    :width: 10%
    :align: center

.. note:: 
    Other than AFCI or GFCI circuit breaker, you need to avoid the surge protector, power strip, and UPS, Uninterrupted Power Supply. Those devices will filter the high frequency transpassing which the power line communication depends on.

Outdoor wireless access point
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If your patio is not shedded or the power line communication was not the best choice. You can choose to install an outdoor access point.
 
There are 2 different choices of the outdoor wireless access points from TP-Link, the omni-directional EAP outdoor access points (EAP225-Outdoor and EAP110-Outdoor), and the directional CPE outdoor access points (CPE210, CPE510, and CPE710). All outdoor wireless access points come with waterproof housing which can be exposed with cover or not.

Omni-directional EAP outdoor wireless access points
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
The EAP Outdoor wireless access points are part of Omada SDN business network. You can control the indoor and outdoor network with the same Omada SDN controller. Or, you can use the Omada outdoor EAP as a standalone wireless access point without a controller. Two of the models are available:
 
* `EAP110-Outdoor 2.4GHz N300 Outdoor Wireless Access Point`_ |ExtLink|
* `EAP225-Outdoor dual-band AC1200 Outdoor Wireless Access Point`_ |ExtLink|

.. _EAP110-Outdoor 2.4GHz N300 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/ceiling-mount-access-point/eap110-outdoor/

.. _EAP225-Outdoor dual-band AC1200 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/ceiling-mount-access-point/eap225-outdoor/

.. note:: 
   There are more features available with the EAP working in controller mode. If you do have a good indoor EAP wireless signal right outside of the house, it is possible to establish a wireless mesh network from inside your house to outdoor area. For more information, please reference to the `Omada SDN Set Up Guide`_ |ExtLink|.

.. _Omada SDN Set Up Guide: https://omada-sdn.readthedocs.io/en/latest/

.. image:: /images/eap225_patio.png
    :width: 80%
    :align: center

Set up the EAP Outdoor wireless access point is easy. There is a PoE injector that comes with the package. Plug one end of the network cable to the Outdoor EAP and plug in to the **PoE** port on the PoE injector with the other end of the network cable. Prepare another network cable connecting the network port of the PoE injector to your home gateway.

.. note:: 
   check up this `how to guide`_ for detailed steps setting up the EAP in standalone mode.

.. _how to guide: https://omada-sdn.readthedocs.io/en/latest/how_to/eap_onboarding.html

The coverage of the wireless can be 100 meter (300 feet) radius from the access point.

.. image:: /images/eap225-coverage.png
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


Directional outdoor wireless access points
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
The CPE Outdoor wireless access points are part of Pharos long distance wireless bridge products. You can also use it to extend the signal around your house if the beam width coverage is good to you:
 
* `CPE210 2.4GHz N300 Outdoor Wireless Access Point`_ |ExtLink|
* `CPE510 5GHz N300 Outdoor Wireless Access Point`_ |ExtLink|
* `CPE710 5GHz AC867 Outdoor Wireless Access Point`_ |ExtLink|

.. |ExtLink| image:: /images/External_Link.png
                     :width: 10 px

.. _CPE210 2.4GHz N300 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/outdoor-radio/cpe210/

.. _CPE510 5GHz N300 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/outdoor-radio/cpe510/

.. _CPE710 5GHz AC867 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/outdoor-radio/cpe710/

The CPE Outdoor wireless access point provides a strong transmitting signal as well as a high  receiving sensitivity. Building a wireless bridge with two identical CPEs can have optimal range and performance. When install only one CPE to extend the wireless range, the communication range will be decided by the weaker transmitter, usually, your wireless client such as a laptop or a cell phone.

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

Choose the Outdoor CPE which has a good coverage and the best wireless gain for your project.

.. image:: /images/cpe_coverage.png
    :width: 80%
    :align: center

The CPE710 access point comes with a feed antenna and a reflective dish. You can install the access point with or without the reflective dish. The reflective dish can refocus the wireless signal to your remote client with concentrated power. If you use the CPE710 in the near site, just around your house, you can remove the reflective dish. However, the direction of the radio waves is opposite.

.. image:: /images/cpe710-feed-mode.png
    :width: 80%
    :align: center

Remote site network expansion (more than 100 meter or 300 feet and up to 18 miles)
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
   how_to/index
   use_case/index
