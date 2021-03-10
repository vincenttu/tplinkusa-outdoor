How to build a CPE wireless bridge
==================================

The easy way to build a wireless bridge is to set one of the CPE works in the access point mode and the other CPE as a client. You can enable the **Lock AP** to build the one to one relationship for security and interference resisting purpose.

A complete setup involves 

* Planning
* CPE settings
* Physical installation

Planning
--------

To set up a long distance wireless bridge, you need to make sure there is a clean Fresnel zone between the CPEs. The most easy way to avoid the trees or fences in the Fresnel zone is to raise up the antenna/CPE.

..note::
    The wireless bridge may still work with partial clean line-of-sight, it is hard to estimate the performance on paper. You need to do an on-site survey to verify if it works.

CPE Settings
------------

It is suggested that you open the box, upgrade them to the latest firmware and set up the network before you go for the physical installation. When you go physical installation, you can then focus on how to align two CPEs facing each other.

Physical Installation
---------------------

There is a plastic zip tie that comes with the package.  You can replace it with a metal one if you expect the weather condition to be more severe. Set the CPE set to access point mode as the radio source and observe the signal strength on the other CPE set to client mode.
Log in to the PharOS and check the radio status. Adjust the aiming angles on both CPEs to get the best signal strength.

.. image:: /images/cpe_alignment.png
    :align: center
    :width: 70%

Grounding
---------

Grounding is extremely important especially for outdoor devices. The Pharos CPEs have a grounding point for easy connection to the ground wire. 

.. image:: /images/cpe_grounding.png
    :align: center

If you do not have a separate grounding point, you can still make the ground connection through the shielded twisted pair network cable, STP. The network module on the CPE can ground through the STP cable, to the PoE injector and to the ground wire on the mains power ground. Please make sure your AC power source grounding is properly set up.

.. image:: /images/cpe_stp.png
    :align: center


Video Guide
-----------

A complete set up video guide is available here:

.. raw:: html

    <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/ISUSlTcgWks" frameborder="0" allowfullscreen></iframe>