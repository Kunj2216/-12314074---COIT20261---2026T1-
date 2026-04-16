Week 04 Tutorial Report – COIT20261

In this week’s tutorial, I worked on understanding how routing works in a network using GNS3.

For the first task, I created a network with multiple Linux hosts, a router, and a switch. I configured IP addresses for each device and made sure they were in the correct subnets. I enabled packet forwarding on the router and disabled it on the hosts. After starting all the nodes, I checked the routing tables using commands and tested connectivity using ping. This helped me understand how data moves between different networks through a router.

In the second task, I explored dynamic routing using OSPF with a pre-configured setup. I used different FRR commands to check neighbour routers and routing tables. I also used traceroute to see the path packets take between hosts. Then, I simulated a network issue by disconnecting a link and observed how OSPF automatically found a new path. This showed how dynamic routing can adjust to changes in the network.

Overall, this tutorial helped me better understand routing tables, packet forwarding, and how dynamic routing protocols like OSPF work in real scenarios.
<img width="720" height="593" alt="network" src="https://github.com/user-attachments/assets/2052595f-4a3e-4a0b-83f0-84a0df3b6094" />
<img width="1898" height="580" alt="ping " src="https://github.com/user-attachments/assets/05b93a29-4d1a-408c-bf5f-9551460f191a" />
<img width="1024" height="406" alt="ping 2" src="https://github.com/user-attachments/assets/df3d054f-fd9a-42c1-8404-735e7ce18972" />
<img width="792" height="321" alt="router" src="https://github.com/user-attachments/assets/116da446-d3a3-4869-b325-e9b86d058501" />
