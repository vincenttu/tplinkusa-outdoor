Outdoor Wireless Example : Remote Camera
========================================

You may have a far away grassland and you want to monitor your cattles there. You may have a parking lot that needs to be monitored on the other size of the building. The easiest way of sending back the pictures is using wireless.

One way or two way communication?
----------------------------------------

Most of the IP cameras send pictures using TCP two way communication by default. Some of the cameras can be set to UDP for one way communication. If you are setting up the camera with UDP communication, you need a strong signal casting from the camera. If you are using the default TCP two way communication, you need strong signals both from and to the camera.

.. image:: /images/uc_camera_connection.png
    :width: 80%
    :align: center

.. note::
	Please reference the `How to calculate the wireless range`_ for requirements of the equipment each way. When doubt, use a pair of the same CPE to build a wireless bridge for the best performance.

.. _How to calculate the wireless range: wireless_range.html

On the camera
----------------------------------------

You can set up a Pharos CPE side by side to the camera using the network port on the PoE injector connecting two devices together. You can set up this CPE works in client mode (most of the time) or in access point mode and connects to the access point or client on the other end.


Installation
------------

* Reference `how to set up a CPE`_ for detail instructions on the CPE set up.
* Remember using a shielded Ethernet cable to connect to the access point and ground the PoE injector proper to provide the best lighting protection.

.. _how to set up a CPE: how_to/cpe_onboarding.html
