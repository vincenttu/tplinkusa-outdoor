How to set up an EAP in standalone mode
=======================================

The Omada EAP can work in controller mode or standalone mode. You can set up and use the EAP as a simple access point without a controller.

.. table:: TP-Link Outdoor Omada EAPs
    :align: center

    +------------+----------------+-----------------+
    | Model      | EAP110-Outdoor | EAP225-Outdoor  |
    +============+================+=================+
    | Frequency  | 2.4GHz         | 2.4GHz and 5GHz |
    +------------+----------------+-----------------+
    | Class      | N300           | AC1200          |
    +------------+----------------+-----------------+

Network topology
----------------

The Omada EAP has a built-in DHCP client enabled by default. It can get the IP address from the home gateway dynamically. Connect the EAP to the PoE injector that comes with the product, plug in to the PoE port. Connect the LAN port of the PoE injector to the home gateway. Power on the EAP.

.. image:: /images/eap_topology.png
    :width: 80%
    :align: center

Set up wizard
-------------

On your computer, search for the SSID TP-Link_xxxx and connect to it. No password was required from factory default. Make sure your computer can get the gateway GUI or Internet. Enter **http://tplinkeap.net** in your browser to get the EAP login page.

.. image:: /images/eap_225_login.png
    :width: 80%
    :align: center

Enter **admin** as the username and **admin** again for the password to login to the set up GUI. Change the user name and password before you proceed to change other settings.

.. image:: /images/eap_new_account.png
    :width: 60%
    :align: center

Follow the setup wizard to enter the SSID and password and save the settings.

.. image:: /images/eap_wireless_setup.png
    :width: 60%
    :align: center