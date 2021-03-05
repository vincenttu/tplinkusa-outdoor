How to calculate the wireless range
===================================

A good radio power is required for a successful radio communication. The original emitting radio power was usually marked as Tx power with the unit in dBm. The attached antenna enhance the radio wave with the unit in dBi. The radio wave travels to the destination with attenuation. Gained with the receiving antenna again and finally reaching the receiver. If the receiver sensitivity is good enough, the signal can be successfully transmitted. 

.. image:: /images/FSPL_Allowance.png

The transmitting power, receiving sensitivity, and antenna gains are stable or maneuverable. But, the path loss can be affected by the equipment setup, blockers, such as glass or wall,  reflection, deflection or other environmental factors. It is hard to estimate the path loss if the path condition is complicated. Usually, we will clear up the factors of attenuation and then make the range estimation as accurate as possible. Assume the transmitter and the receiver are face to face with no obstacles in between and neglect the factors of the reflection and deflection, then the major factor of the path loss is the Free Space Path Loss, FSPL. And we usually set other variable factors to the margin of the signal loss.

.. note:: 
   **Free Space Path Loss:** The path loss in free space is a radio wave  decreases with distance by the inverse square law. The same amount of power spreads over an area proportional to the square of distance from the source. `External Reference`_ |ExtLink|

   |FSPL|
   
   And the formula can be expressed like this:

   .. image:: /images/FSPL_formula.png

   
.. |FSPL| image:: /images/FSPL.png

.. _External Reference: https://en.wikipedia.org/wiki/Free-space_path_loss

.. |ExtLink| image:: /images/External_Link.png
    :width: 10 px

Device characteristics
----------------------

Here's the list of the device radio characteristics.

+-----------+--------+--------+--------+----------------+----------------+------------+
| Model     | CPE210 | CPE510 | CPE710 | EAP225-Outdoor | EAP110-Outdoor | Cell Phone |
+===========+========+========+========+================+================+============+
| Beamwidth | 65°    | 45°    | 9°     | 360°           | 360°           | 360°       |
+-----------+--------+--------+--------+----------------+----------------+------------+
| Antenna   | 9 dBi  | 13 dBi | 23 dB  | 3 dBi          | 4dBi           | 2 dBi      |
+-----------+--------+--------+--------+----------------+----------------+------------+
| Tx Power  | 25 dBm | 26 dBm | 27 dBm | 30 dBm         | 30dBm          | 10 dBm     |
+-----------+--------+--------+--------+----------------+----------------+------------+

The Outdoor EAP has omni-directional antennas with 360° radio emitting directions. The Outdoor CPE access points are focused on one direction. The radio characteristics of a cell phone is just an example. You can change this value in following calculations. 

To find out the communication range, we can figure out the FSPL allowance and then translate the FSPL into the distance. We can rewrite the FSPL formula like this:

.. image:: /images/FSPL_Formula_2.png
    :width: 70%

Where the d is the distance in meters and the f is the frequency in MHz.

Calculate the range from the outdoor AP to a cell phone
-------------------------------------------------------

With all the formula and parameters, let’s calculate the estimated wireless range.

From the AP to the cell phone
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

A good receiving sensitivity on the cell phone is assumed to be -75dB.

+----------------+-----------+----------+--------------+--------+--------+--------------+-------------+-----------+
| Model          | Frequency | Tx Power | Antenna Gain | FSPL   | Margin | Antenna Gain | Sensitivity | Distance  |
+================+===========+==========+==============+========+========+==============+=============+===========+
| CPE210         | 5,000MHz  | 25 dBm   | 9 dBi        | 91 dB  | 20 dB  | 2 dBi        | -75 dB      | 352.6 m   |
+----------------+-----------+----------+--------------+--------+--------+--------------+-------------+-----------+
| CPE510         | 5,000MHz  | 26 dBm   | 13 dBi       | 96 dB  | 20 dB  | 2 dBi        | -75 dB      | 301.0 m   |
+----------------+-----------+----------+--------------+--------+--------+--------------+-------------+-----------+
| CPE710         | 5,000MHz  | 27 dBm   | 23 dBi       | 107 dB | 20 dB  | 2 dBi        | -75 dB      | 1,067.9 m |
+----------------+-----------+----------+--------------+--------+--------+--------------+-------------+-----------+
| EAP225-Outdoor | 5,000MHz  | 30 dBm   | 3 dBi        | 90 dB  | 20 dB  | 2 dBi        | -75 dB      | 314.3 m   |
+----------------+-----------+----------+--------------+--------+--------+--------------+-------------+-----------+
| EAP110-Outdoor | 2,400MHz  | 30 dBm   | 4 dBi        | 90 dB  | 20 dB  | 2 dBi        | -75 dB      | 150.8 m   |
+----------------+-----------+----------+--------------+--------+--------+--------------+-------------+-----------+

From the cell phone to the AP
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+----------------+-----------+----------+--------------+--------+--------+--------------+-------------+----------+
| Model          | Frequency | Tx Power | Antenna Gain | FSPL   | Margin | Antenna Gain | Sensitivity | Distance |
+================+===========+==========+==============+========+========+==============+=============+==========+
| CPE210         | 5,000MHz  | 10 dBm   | 2 dBi        | 91 dB  | 20 dB  | 9 dBi        | -80 dB      | 111.5 m  |
+----------------+-----------+----------+--------------+--------+--------+--------------+-------------+----------+
| CPE510         | 5,000MHz  | 10 dBm   | 2 dBi        | 96 dB  | 20 dB  | 13 dBi       | -80 dB      | 84.8 m   |
+----------------+-----------+----------+--------------+--------+--------+--------------+-------------+----------+
| CPE710         | 5,000MHz  | 10 dBm   | 2 dBi        | 107 dB | 20 dB  | 23 dBi       | -80 dB      | 268.2 m  |
+----------------+-----------+----------+--------------+--------+--------+--------------+-------------+----------+
| EAP225-Outdoor | 5,000MHz  | 10 dBm   | 2 dBi        | 90 dB  | 20 dB  | 3 dBi        | -80 dB      | 55.9 m   |
+----------------+-----------+----------+--------------+--------+--------+--------------+-------------+----------+
| EAP110-Outdoor | 2,400MHz  | 10 dBm   | 2 dBi        | 90 dB  | 20 dB  | 4 dBi        | -80 dB      | 26.8 m   |
+----------------+-----------+----------+--------------+--------+--------+--------------+-------------+----------+

Frequent Asked Question
=======================
