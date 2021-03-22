Outdoor Wireless Example : - High school football field
=======================================================

.. image:: /images/uc_football.png
    :width: 100%
    :align: center

At the school football stadium, you may want to provide basic Internet access to all the audiences, to share the pictures or the videos. Most of the time, the football stadium is away from the office and has no network cable buried when it was built. How can we provide the network services to the bench area?

To the audiences
----------------

Separate the bench areas in different sections of services. In this example, there are 2 major bench areas and each area can be covered by 250 feet radius from the stadium lighting poles. We can mount a 360° EAP access point for the service. Since the uplink speed is up to 300Mbps, we can simply deploy an EAP110-Outdoor here.

.. image:: /images/uc_football_eap.png
    :width: 80%
    :align: center

To the office
-------------

The distance from the stadium lighting poles to the office is about 1,200 feet and has a good line-of-sight condition. We can use CPE510 to build a 5GHz uplink. Since two of the stadium lighting poles are within 45° angle looking from the office, we can set up one CPE510 outside of the office as an access point connecting to two CPE510 on the stadium lighting poles set up as clients.

.. image:: /images/uc_football_cpe.png
    :width: 80%
    :align: center

Installation
------------

The network topology looked like this:

.. image:: /images/uc_football_topo.png
    :width: 80%
    :align: center

* Reference `how to set up a CPE`_ or  `how to set up an EAP`_ for detail instructions on access point set up.
* Remember using a shielded Ethernet cable to connect to the access point and ground the PoE injector proper to provide the best lighting protection.

.. _how to set up a CPE: how_to/cpe_onboarding.html

.. _how to set up an EAP: how_to/eap_onboarding.html