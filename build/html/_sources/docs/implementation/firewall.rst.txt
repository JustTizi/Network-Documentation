Firewall
--------



.. seealso:: For more information about firewall configuration on MikroTik devices, visit `MikroTik's Firewall documentation <https://help.mikrotik.com/docs/spaces/ROS/pages/48660574/Filter>`_

To secure the routers from unauthorized access, we have to configure some firewall rules. These are used to filter through traffic coming into the router. 

*SepsiLab:*

.. image:: ../../img/fw/sepsilab_fw.png
    :alt: Firewall settings of router SepsiLab

* **Rule 1**: FastTrack established and related connections in the forward chain for faster data throughput, the firewall will work with new connections only.
* **Rule 2**: Allow established and related connections in the input chain for traffic targeting the router.
* **Rule 3**: Allow established and related connections in the forward chain for traffic passing through the router.
* **Rule 4**: Allow incoming WireGuard protocol (UDP) traffic on the input chain.
* **Rule 5**: Allow input traffic from the WireGuard subnet (10.253.3.0/24).
* **Rule 6**: Allow input traffic from local interfaces.
* **Rule 7**: Allow forwarded traffic from the WireGuard subnet (10.253.3.0/24).
* **Rule 8**: Allow forwarded traffic from local interfaces.
* **Rule 9**: Drop all other traffic in the forward chain.
* **Rule 10**: Drop all other traffic in the input chain.

*sagan:*

.. image:: ../../img/fw/sagan_fw.png
    :alt: Firewall settings of router sagan

* **Rule 1**: Allow forwarded traffic from router SepsiLab to router Gala
* **Rule 2**: Allow forwarded traffic from router Gala to router SepsiLab
