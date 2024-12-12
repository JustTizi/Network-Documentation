Test results
------------



And finally with all of this configured, we have connectivity between the routers.

*Ping test from local device on SepsiLab network to Sagan:*

.. image:: ../../img/tests/pc_sagan_ping.png
    :alt: Ping test from local device on SepsiLab network to Sagan

*Traceroute test from local device on SepsiLab network to Sagan:*

.. image:: ../../img/tests/pc_sagan_trace.png
    :alt: Traceroute test from local device on SepsiLab network to Sagan

*Ping test from local device on SepsiLab network to Gala:*

.. image:: ../../img/tests/pc_gala_ping.png
    :alt: Ping test from local device on SepsiLab network to Gala

*Traceroute test from local device on SepsiLab network to Gala:*

.. image:: ../../img/tests/pc_gala_trace.png
    :alt: Traceroute test from local device on SepsiLab network to Gala


You might have noticed that the Traceroute results only show the routers in the VPN network (namely SepsiLab, Sagan and Gala). This actually means that our VPN tunnel is encrypting the data properly. 

If the data wasn't encrypted, the intermediate hops, like the ISP hops, would be giving us a reply on the ICMP request. In reality, it's not sending anything back because the hops can't read the request. With this, we can safely say that our data is securely getting transferred.