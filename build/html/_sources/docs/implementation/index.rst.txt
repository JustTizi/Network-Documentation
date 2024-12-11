Implementation
==============

In order to be able to have the MQTT data arrive inside the SepsiLab network, multiple settings had to be configured on the routers we have available. 

I'll be going over the following points:

* `GNS3`_
* `WireGuard`_
* `NAT`_
* `Firewall`_


.. include:: ./gns.rst

.. include:: ./wireguard.rst

.. include:: ./nat.rst

.. include:: ./firewall.rst

And finally with all of this configured, we have connectivity between the routers.

.. image:: ../../img/test.png
    :alt: Ping test from device on SepsiLab network to Gala