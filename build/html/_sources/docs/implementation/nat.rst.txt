NAT
---

.. seealso:: For more information on NAT, check the `Wikipedia page <https://wikipedia.org/wiki/Network_address_translation>`_

After setting up our WireGuard interface, we can set up our NAT.

*SepsiLab:*

.. image:: ../../img/nat/sepsilab_nat.png
    :alt: NAT settings of router SepsiLab

*sagan:*

.. image:: ../../img/nat/sagan_nat.png
    :alt: NAT settings of router sagan

For our setup, I've opted to use the `Masquerade functionality <https://help.mikrotik.com/docs/spaces/ROS/pages/3211299/NAT#NAT-Masquerade>`_ of the MikroTik devices. This setting is similar to PAT and will allow us to use devices on our local network to connect over the VPN tunnel as well.

On router sagan, we do not need the `Masquerade functionality`_ for the WireGuard interface, as such it's only configured for the WAN interface.