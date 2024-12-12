End result
----------

Now the question remains, what are we going to implement to make this work?

We will be setting up a WireGuard VPN network on our MikroTik routers, with a hub-and-spoke topology. This means each spoke router will be able to connect to the central hub router, allowing for secure communication between remote sites.

So what do we need to do?

    #. Have at least one public IP address (for the hub)
    #. Configure the WireGuard interface and peers
    #. Set up NAT to communicate from our local devices over the internet and WireGuard tunnel
    #. Configure a firewall to secure our network

After we've done all of that, we should be able to connect over the VPN tunnel.

With that out of the way, let's see how we can set this up ourselves.