Outdoor Wireless Example : Yacht Club
=====================================

Here is an outdoor wireless coverage example. A yacht club wants to provide Internet services to all yacht owners. Yacht owners need Internet connections to browse the Internet, access emails and watch Netflix videos. Wireless access points can be mount on the wall of the buildings.

.. image:: /images/uc_yacht_club.png
    :align: center
    :width: 70%

According to the recommendation of the Netflix.com, the bandwidth requirements are:

.. table:: Netflix video streaming bandwidth requirements
    :align: center

+----------+-----------+
| Service  | Bandwidth |
+==========+===========+
| Minimum  | 0.5Mbps   |
+----------+-----------+
| SD Video | 3.0Mbps   |
+----------+-----------+
| HD Video | 5.0Mbps   |
+----------+-----------+
| Ultra HD | 25Mbps    |
+----------+-----------+

A reasonable bandwidth allocation for each boat is 6Mbps for all the services. Because the wireless communication shares the total bandwidth, each boat can get more than 6Mbps connection when the total number of clients is low and gets allocated bandwidth when the number of clients reaches the capacity of the plan.

Plan 1 : minimum access points
------------------------------

A simple 3 access points plan with EAP225-Outdoor can cover all the boats. All 3 access points can be mounted on the exterior walls of the club and provide services to 11 ~ 30 boats. The planned bandwidth capacity 30 x 6Mbps = 180Mbps can be easily handed by EAP-225-Outdoor.

.. image:: /images/uc_yacht_club_3.png
    :align: center
    :width: 70%

The access point C has a 320 feet radius service range to 30 boats. The wireless path is longer and the loading is heavier. The customer has some concerns on it. It is possible to make the service area smaller to distribute the load. So, we then break the lower single access point service area to be served by 3 EAP225-Outdoor. 

Plan 2 : with all EAPs for easy management
------------------------------------------

.. image:: /images/uc_yacht_club_5.png
    :align: center
    :width: 70%

When an access point can be hard wired to the network, it is easier to maintain and the hard wire provides the separate bandwidth for uplink than wireless downlink. In this 5 EAPs wireless plan, you can see the access point E is not attached to the building. It was planned to be mounted on the sidewalk lamp pole and wirelessly meshed to the main network. This installations provides a great flexibility when choosing the installation spot.

Plan 3 : balance the service group size with minimum network management
-----------------------------------------------------------------------

After the discussion between the installer and the landlord. They decided that they want to break the clients in smaller service groups for better bandwidth and network management, at the same time, they want to attach the access points on the main building for easy installation. Therefore, the plan was modified again mixing the CPE510 in this service plan. In this service plan, we leave the first three EAP225-Outdoor access points to service upper part of the boats and use two CPE510 (45° beam width) to service the 4th and 5th group, so the total number of the clients to each access point is lower and the bandwidth plan for each boat can be upgraded.

.. image:: /images/uc_yacht_club_cpe.png
    :align: center
    :width: 70%

Installation
------------

Since both CPEs and EAPs work in access point mode, the customer decided to set them one by one in standalone mode. You can reference the how to section of this document about how to set up EAP and CPE as an access point.




