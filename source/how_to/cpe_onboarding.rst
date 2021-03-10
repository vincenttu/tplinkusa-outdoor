How to set up a CPE
===================

The TP-Link Pharos CPEs are the outdoor wireless access points designed for long range point to point communications.

**Pharos**
	Is the name of the product line for long range wireless bridge. 

**PharOS**
	Is the name of the cross model firmware. All Pharos products share the same hardware architecture and the same firmware for easy management and are named PharOS.

**Pharos Control**
	Pharos Control is a controller to control multiple Pharos products. It maintains location information and has TDMA, Time Division Multiple Access, management features mainly for point to multiple point long range communications. For a single point to point bridge or a single access point, you don’t need the controller to manage the network.

.. table:: TP-Link Pharos CPEs
    :align: center

    +------------+--------+--------+--------+
    | Model      | CPE210 | CPE510 | CPE710 |
    +============+========+========+========+
    | Frequency  | 2.4GHz | 5GHz   | 5GHz   |
    +------------+--------+--------+--------+
    | Class      | N300   | N300   | AC867  |
    +------------+--------+--------+--------+
    | Beamwidth  | 65°    | 45°    | 9°     |
    +------------+--------+--------+--------+
    | Max Paired | 3      | 9      | 18     |
    | Range      | miles  | miles  | miles  |
    +------------+--------+--------+--------+

Log in to the PharOS
--------------------

The Pharos CPE has the default IP at 192.168.0.254/24. To access the PharOS web GUI page, you have to set your computer's IP address within the same subnet such as 192.168.0.10.

.. note::
    * `How to set up static IP on Windows 10`_

    * `How to set up static IP on macOS`_

.. _How to set up static IP on Windows 10: win10_static_0_10.html
.. _How to set up static IP on macOS: mac_static_0_10.html

When you first time log in to the PharOS, enter the user name **admin** and password **admin**.

.. image:: /images/PharOS.png
    :align: center

You have to change your user name and password on the first time login. Set up account information and then login again.

Set up CPE as an access point
-----------------------------

The CPE can work in different operation modes, it is set to access point mode by default. You can simply change the wireless settings to complete the setup.

Choose the **WIRELESS** tab. Then in the **Wireless AP Settings** section, change the SSID name, choose **WPA-PSK** security mode, and then enter the password in PSK Password. (PSK stands for pre-shared key). Then click **Apply**.

.. image:: /images/PharOS.png
    :align: center

The CPE is an enterprise product and has separated stages of working image, one is running image and one is boot image. After you change the wireless settings, you have to click the **Save** again to save the running configurations to the boot configuration. Otherwise, the settings will not be remembered after the power cycle.

.. image:: /images/PharOS_save.png
    :align: center

Set up CPE as an client
-----------------------

To build a wireless bridge, you can set one of the CPE as the access point and then the second CPE as a client connecting to the first access point. To set up a CPE as an client, you have to change the **operation mode**.

Choose the **Client** in the **Operation Mode**. 

.. image:: /images/PharOS_modes.png
    :align: center

Click **Yes** to confirm the mode change.

.. image:: /images/PharOS_mode_change.png
    :align: center

In **Wireless Client Settings** section, enter the SSID and password, then click on **Apply**

.. image:: /images/PharOS_client.png
    :align: center

Click on the **Save** to save the settings.

.. image:: /images/PharOS_save.png
    :align: center

.. note::
    You can click on the **Survey** to search for the access point. Check the access point and then click **Connect** to copy the SSID to the settings page.

    .. image:: /images/PharOS_survey.png
        :align: center
        :width: 70%