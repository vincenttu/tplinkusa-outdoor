.. TP-Link USA Outdoor Solution Guide master file

TP-Link USA Outdoor Solution Guide
==================================

Many TP-Link products can extend the Internet coverage from your home or business to outdoor areas. This Solutions Guide will introduce the various ways to expand your indoor network to outdoor spaces, including a backyard, a remote barn or guest house, a dock or yacht club, campgrounds, and other large outdoor areas.

How far do you want to go?  Near or remote site 
-----------------------------------------------

Depending on how far from the house or building you want to extend your wireless connection determines what solution will best meet your needs. There are many possible solutions to expand the network just around your house's outdoor perimeter within 100 meters (300 feet).  A network extension to a back house or secondary workshop farther than 300 feet will need a point-to-point wireless bridge to re-broadcast the signal on to the remote location. Each outdoor application has different environmental requirements; it is essential to review these requirements to determine the best Outdoor Solution for your needs. 

Near Site Network Extension (up to 100 meters or 300 feet) 
----------------------------------------------------------

If you have strong indoor wireless, you can easily extend your network to the patio, pool area, or large yard. While wireless signals can penetrate glass windows, it is much harder for signals to penetrate wire-filled stucco walls. These metal wires are perfect for preventing wireless interference inside your home by blocking signals from the outside. While ensuring better protection for your home, stucco walls can stop the wireless transmission from the indoors to the outdoors. 

You can choose the power line communication adapters help extending your network out of your house. Or, you need to put a network wire through the exterior wall to get the data out. 

.. image:: /images/mesh_wires.jpeg
    :width: 50%
    :align: center

Near site solution 1: Power line communication
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If you have a covered patio or waterproof electric box, you can extend the network with TP-Link's power line adapters. The TL-WPAxx Series Power Line Wireless Adapter Kit is the easiest solution and includes two power line communication adapters. One adapter installed indoors relays the data from the network cable to the power line, while the second adapter broadcasts the WiFi signal to your computer or phone. 

.. image:: /images/PLC-patio.png
    :width: 60%
    :align: center

Plug-in the first power line (PLC) adapter to a power outlet near the home router. Now, connect the network port on the PLC adapter to the router with the network cable. Finally, plug the second PLC adapter (with the wireless features) into the power socket on your patio or in the waterproof box. 

.. note:: 
    Both PLC adapters are rated as indoor devices. If there is any chance that the PLC adapter on the patio could be splashed by water or exposed to weather, please provide appropriate water/weather protection for it. 

PLC for the back house/office 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If you have, or recently added, a back yard office/shed, back house, or summer pool house, you may be ready to extend the internet to the area. If there is power to the isolated building, there is a good chance the main house's power line is buried. If you do have a power line run to the building but no data wiring run, you can easily extend your network using the buried power line. 

.. image:: /images/PLC-backyard_office.png

To also use the power line as a data line for the back house/office, you need to find the direct connect electric loop connecting your home and the back yard office. In most installations, the power line is connected between two circuit breaker panels. One on the main house and one on the back house/office. Therefore, the PLC adapters must communicate to each other through at least two (2) circuit breakers. With the latest technology, the data communication can pass through a simple breaker, but not the AFCI or GFCI type circuit breakers. Find the close by power socket to the power panel to build the best communication that you can have. 


.. image:: /images/AFCI_Breaker.png
    :width: 10%
    :align: center

.. note:: 
    Other than AFCI or GFCI circuit breaker, you need to avoid the surge protector, power strip, and UPS, Uninterrupted Power Supply. Those devices will filter the high frequency signal which the power line communication relies on.

Near site solution 2: Outdoor wireless access point
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If your patio is not enclosed or the power line method is not the best option for you, it is advisable to install an outdoor access point. 
 
TP-Link offers two (2) different outdoor wireless access points, the omni-directional EAP outdoor access points (EAP225-Outdoor and EAP110-Outdoor) and the directional CPE outdoor access points (CPE210, CPE510, and CPE710). All outdoor wireless access points come with waterproof housing, which can be placed with a cover or not.  

1. Omni-directional EAP outdoor wireless access points
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
The EAP Outdoor wireless access points are part of the Omada SDN business network. With Omada, you can control the indoor and outdoor network with the same Omada SDN controller. Or use the Omada outdoor EAP as a standalone wireless access point without a controller.  
Two available models: 
 
* `EAP110-Outdoor 2.4GHz N300 Outdoor Wireless Access Point`_ |ExtLink|
* `EAP225-Outdoor dual-band AC1200 Outdoor Wireless Access Point`_ |ExtLink|

.. _EAP110-Outdoor 2.4GHz N300 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/ceiling-mount-access-point/eap110-outdoor/

.. _EAP225-Outdoor dual-band AC1200 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/ceiling-mount-access-point/eap225-outdoor/

.. note:: 
    There are more features available with the EAP working in controller mode. If you have an excellent indoor EAP wireless signal right outside of the house, it is possible to establish a wireless mesh network from inside the home to the outdoor area. For more information, please refer to the `Omada SDN Set Up Guide`_ |ExtLink|.

.. _Omada SDN Set Up Guide: https://omada-sdn.readthedocs.io/en/latest/

.. image:: /images/eap225_patio.png
    :width: 80%
    :align: center

Setting up the EAP Outdoor wireless access point is quick. Plug one end of the network cable into the Outdoor EAP and plug the other end into the **PoE** port on the included PoE injector. Finally, prepare another network cable to connect the network port of the PoE injector to your home gateway.  

.. note:: 
   check up this `EAP Onboarding How-to Guide`_ for detailed steps setting up the EAP in standalone mode.

.. _EAP Onboarding How-to Guide: https://omada-sdn.readthedocs.io/en/latest/how_to/eap_onboarding.html

The coverage of the wireless can be 100 meter (300 feet) radius from the access point.

.. image:: /images/eap225-coverage.png
    :width: 80%
    :align: center

2. Outdoor wireless mesh networking
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Extending radio signals with outdoor EAP access points is different from the outdoor CPE. The only outdoor EAP that supports the wireless extender feature is the EAP225-Outdoor. To extend the radio signal, you will set up a wireless mesh network. The wireless mesh network requires a controller to coordinate the traffic, so a basic topology of an outdoor EAP mesh network can be like this. 

.. image:: /images/eap225-mesh.png
    :width: 80%
    :align: center

The EAP225-Outdoor mesh can wirelessly link back to the network up to 3 hops. As you can see, a complex dock or yacht club wireless deployment is achieved easily with the outdoor EAP mesh network. 

.. figure:: /images/eap225-yacht.png
    :width: 80%
    :align: center
    
    A yacht club wireless deployment example with EAP225-Outdoor


3. Directional outdoor wireless access points
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
The CPE Outdoor wireless access points are part of Pharos long-distance wireless bridge products. You can also use outdoor APs to extend the signal around your house if the beam width coverage is suitable to you: 
 
* `CPE210 2.4GHz N300 Outdoor Wireless Access Point`_ |ExtLink|
* `CPE510 5GHz N300 Outdoor Wireless Access Point`_ |ExtLink|
* `CPE710 5GHz AC867 Outdoor Wireless Access Point`_ |ExtLink|

.. |ExtLink| image:: /images/External_Link.png
                     :width: 10 px

.. _CPE210 2.4GHz N300 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/outdoor-radio/cpe210/

.. _CPE510 5GHz N300 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/outdoor-radio/cpe510/

.. _CPE710 5GHz AC867 Outdoor Wireless Access Point: https://www.tp-link.com/us/business-networking/outdoor-radio/cpe710/

The CPE Outdoor wireless access point provides a strong transmitting signal as well as a high receiving sensitivity. Building a wireless bridge with two identical CPEs can give optimal range and performance. When installing only one CPE device to extend the wireless range, the weaker transmitter will decide the communication range, this is usually your wireless client such as a laptop or a cell phone. 

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

The CPE710 access point comes with a feed antenna and an optional reflective dish.  Use the reflective dish when sending your signal longer ranges to refocus the wireless signal to your remote client with concentrated power. If you use the CPE710 just around your house, you can remove the reflective dish. However, remember the direction of the radio waves is the opposite (see graphic). 

.. image:: /images/cpe710-feed-mode.png
    :width: 80%
    :align: center

Remote site network expansion (more than 100 meter or 300 feet and up to 18 miles)
----------------------------------------------------------------------------------

If you have a barn or back house, a remote surveillance camera, or a video doorbell on the vineyard entrance, and the distance from your home is more than 300 feet, you can use the outdoor CPE to build a wireless bridge to further expand the network for miles. 

You can also broadcast the wireless signals with an additional wireless access point on the remote site when necessary. 

.. image:: /images/cpe-dock_house.png
    :width: 80%
    :align: center

.. toctree::
   :maxdepth: 2
   :caption: Document Index:

   wireless_range
   how_to/index
   use_case/index
