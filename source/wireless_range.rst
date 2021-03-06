How to calculate the wireless range
===================================

A good radio power is required for a successful radio communication. The original emitting radio power was usually marked as Tx power with the unit in dBm. The attached antenna enhance the radio wave with the unit in dBi. The radio wave travels to the destination with attenuation. Gained with the receiving antenna again and finally reaching the receiver. If the receiver sensitivity is good enough, the signal can be successfully transmitted. 

.. image:: /images/FSPL_Allowance.png

The transmitting power, receiving sensitivity, and antenna gains are known parameters when you choose the devices. The path loss can be the only variable. The path loss can be contributed by the equipment setup, transmitting medium, such as glass or wall,  reflection, deflection or other environmental factors. It is hard to estimate the path loss when the path condition is complicated. In practice, we will choose the clear line-of-sight wireless path to avoid the possible path loss. Then, we can assume the transmitter and the receiver are face to face with no obstacles in between and neglect the factors of the reflection and deflection. Under this condition, the major factor of the path loss is the Free Space Path Loss, FSPL.

The radio waves are directional and guided by the antenna. The CPE access point concentrates the waves in a limited angle of the direction. However, the receiver still cannot receive 100% of the transmitted power. As the distance between the transmitter and receiver increases, the receiving percentage decreases. The detailed calculation can be expressed by FSPL formula.

.. note:: 
   **Free Space Path Loss:** The path loss in free space is a radio wave  decreases with distance by the inverse square law. The same amount of power spreads over an area proportional to the square of distance from the source. `External Reference`_ |ExtLink|

   |FSPL|
   
   And the formula can be expressed like this:

   .. image:: /images/FSPL_formula.png
        :align: center

   
.. |FSPL| image:: /images/FSPL.png 

.. _External Reference: https://en.wikipedia.org/wiki/Free-space_path_loss

Device characteristics
----------------------

Here's the TP-Link outdoor access point wireless characteristics. They are the key factors for good radio signals. On the cell phone, we simply use an average number. If you happen knowing the device you use, you can replace it with the numbers you have.

.. table:: Device Radio Characteristics

    +-----------+--------+--------+--------+-----------+-----------+------------+
    | Model     | CPE210 | CPE510 | CPE710 | EAP225-OD | EAP110-OD | Cell Phone |
    +===========+========+========+========+===========+===========+============+
    | Beamwidth | 65°    | 45°    | 9°     | 360°      | 360°      | 360°       |
    +-----------+--------+--------+--------+-----------+-----------+------------+
    | Antenna   | 9 dBi  | 13 dBi | 23 dB  | 3 dBi     | 4dBi      | 2 dBi      |
    +-----------+--------+--------+--------+-----------+-----------+------------+
    | Tx Power  | 25 dBm | 26 dBm | 27 dBm | 30 dBm    | 30dBm     | 10 dBm     |
    +-----------+--------+--------+--------+-----------+-----------+------------+

The Outdoor EAP has omni-directional antennas with 360° radio emitting directions. The Outdoor CPE access points are focused on one direction.

Calculate the range from the outdoor AP to a cell phone
-------------------------------------------------------

To find out the communication range, we can figure out the FSPL allowance and then translate the FSPL into the distance. We can rewrite the FSPL formula like this:

.. image:: /images/FSPL_Formula_2.png
    :width: 70%
    :align: center

Where the d is the distance in meters and the f is the frequency in MHz.

With all the formula and device parameters, let’s calculate the estimated wireless range.

A good receiving sensitivity on the cell phone is assumed to be -75dB. Sometimes the sensitivity is better or worse and it can be included in the 20dB margin.

.. figure:: images/ap-to-cellphone.png

    Range estimation from an AP to a cell phone


From the table, we can find that the transmission from the outdoor access point to the cell phone. It looks pretty good. But, most of the applications we are using today require two way communications. Let’s take a look at the return path.

.. figure:: images/cellphone-to-ap.png

    Range estimation from a cell phone to an AP

The distance estimation is much shorter because of the radio power provided by the cell phone is usually lower. With a better antenna on the access point, you can still get a better range compare to home wireless routers. The transmit power on the client side can be improved if you have an external wireless adapter on a laptop computer, such as Archer T4U Plus.

.. note:: 
    1. The EAP225-Outdoor is a dual band access point. The 2.4GHz performance is the same as the EAP110-Outdoor and didn’t show on the table separately.
    2. The outdoor AP sensitivities are set to -80dB for easy presentation. The real radio sensitivity is varied in different protocols it runs on. The range of the sensitivities can be -75dB to -95dB.

The range for a pair of Outdoor CPE
-----------------------------------

The maximum range of the CPE wireless bridge was tested in the field and listed below. If you have special environmental conditions, you can use the formula above for better estimation. 

.. table:: Maximum range to a pair of CPE
    :align: center

    +-------+---------+---------+----------+
    | Model | CPE210  | CPE510  | CPE710   |
    +=======+=========+=========+==========+
    | Range | 3 miles | 6 miles | 18 miles |
    +-------+---------+---------+----------+

When you set up a pair of CPE as a wireless bridge. You can set one of the CPE to be the access point and the other CPE as a client to build the bridge. Please reference the the user’s manual for how to set up the CPE.

Outdoor EAP mesh connectivity and maximum range
-----------------------------------------------
    
The EAP225-Outdoor mesh network can be extended up to 3 hops with only the wireless connections. The recommended maximum distance on each hop is 100 meters. So, the maximum mesh coverage will be 400 meters radius area.

.. figure:: /images/uc_mesh_simulation.png
    :align: center
    :width: 70%

    An example of outdoor mesh wireless planning for a paintball battle field

Frequent Asked Questions
------------------------

1. The range estimation was based on clear line-of-sight radio path. What if I have something in between?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Electromagnetic conductors, such as a metal plate, is definitely a major blocker of the radio wave. Other materials have different effects as well. Here’s a list of material and radio attenuation in general. You can put the attenuation in the rangefinder formula for a new estimation.

+-----------------------------+---------------------+-------------------+
| Building Material           | 2.4 GHz Attenuation | 5 GHz Attenuation |
+=============================+=====================+===================+
| Solid Wood Door 1.75"       | 6 dB                | 10 dB             |
+-----------------------------+---------------------+-------------------+
| Hollow Wood Door 1.75"      | 4 dB                | 7 dB              |
+-----------------------------+---------------------+-------------------+
| Interior Office Door        | 4 dB                | 6 dB              |
| w/Window 1.75"/0.5"         |                     |                   |
+-----------------------------+---------------------+-------------------+
| Steel Fire/Exit Door 1.75"  | 13 dB               | 25 dB             |
+-----------------------------+---------------------+-------------------+
| Steel Fire/Exit Door 2.5"   | 19 dB               | 32 dB             |
+-----------------------------+---------------------+-------------------+
| Steel Rollup Door 1.5"      | 11 dB               | 19 dB             |
+-----------------------------+---------------------+-------------------+
| Brick 3.5"                  | 6 dB                | 10 dB             |
+-----------------------------+---------------------+-------------------+
| Concrete Wall 18"           | 18 dB               | 30 dB             |
+-----------------------------+---------------------+-------------------+
| Cubical Wall (Fabric) 2.25" | 18 dB               | 30 dB             |
+-----------------------------+---------------------+-------------------+
| Exterior Concrete Wall 27"  | 53 dB               | 45 dB             |
+-----------------------------+---------------------+-------------------+
| Glass Divider 0.5"          | 12 dB               | 8 dB              |
+-----------------------------+---------------------+-------------------+
| Interior Hollow Wall 4"     | 5 dB                | 3 dB              |
+-----------------------------+---------------------+-------------------+
| Interior Hollow Wall 6"     | 9 dB                | 4 dB              |
+-----------------------------+---------------------+-------------------+
| Interior Solid Wall 5"      | 14 dB               | 16 dB             |
+-----------------------------+---------------------+-------------------+
| Marble 2"                   | 6 dB                | 10 dB             |
+-----------------------------+---------------------+-------------------+
| Bullet-Proof Glass 1"       | 10 dB               | 20 dB             |
+-----------------------------+---------------------+-------------------+
| Exterior Double Pane        | 13 dB               | 20 dB             |
| Coated Glass 1"             |                     |                   |
+-----------------------------+---------------------+-------------------+
| Exterior Single Pane        | 7 dB                | 6 dB              |
| Window 0.5"                 |                     |                   |
+-----------------------------+---------------------+-------------------+
| Interior Office Window 1"   | 3 dB                | 6 dB              |
+-----------------------------+---------------------+-------------------+
| Safety Glass-Wire 0.25"     | 3 dB                | 2 dB              |
+-----------------------------+---------------------+-------------------+
| Safety Glass-Wire 1.0"      | 13 dB               | 18 dB             |
+-----------------------------+---------------------+-------------------+

2. How to place your wireless device for optimal reception and performance?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    
1. Make sure there is no blocker between two wireless devices (Line-of-sight)
2. Adjust outdoor EAP adjustable antennas 90° to each other in a complex environment. Try different angles to get the best reflection and deflection in the radio path.

3. What is Line-of-sight?
~~~~~~~~~~~~~~~~~~~~~~~~~

The electromagnetic line-of-sight defined by a `Fresnel zone`_ |ExtLink|. Other than the line that draws from the center point from one access point to another. Any obstacles falling in the Fresnel zone will be considered a blocker of the radio waves. The easiest way to avoid the blockers is elevating  the antenna. The height of the antenna should be good enough to remove blockers in the Fresnel zone.

.. image:: /images/line-of-sight.png
    :width: 80%
    :align: center

.. _Fresnel zone: https://en.wikipedia.org/wiki/Fresnel_zone

.. |ExtLink| image:: /images/External_Link.png
    :width: 10 px