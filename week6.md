COIT20261 – Network Services and Automation
Week 6 Tutorial Report

This week’s tutorial focused on understanding how devices communicate within and across networks using ARP and default gateways. The activities were completed using a simulated network environment, which helped in visualizing real-world networking concepts.

Task 1: Resolving IP Addresses to Hardware Addresses (ARP)

In this task, a network consisting of four Linux hosts connected via an Ethernet switch was used to study how ARP (Address Resolution Protocol) works.

Initially, the ARP table of Host A was checked using the command ip neigh show. At this stage, the table had very limited or no entries because no communication had taken place yet.

After pinging Host B from Host A, the ARP table was checked again. A new entry appeared showing the mapping between Host B’s IP address and its corresponding MAC (hardware) address. The state of the entry was shown as REACHABLE, indicating successful communication.

Next, Host C was used to ping Host A. When the ARP table of Host A was viewed again, another entry was added for Host C. This demonstrated that ARP dynamically updates its table as devices communicate within the network.

Overall, this task clearly showed how ARP helps devices identify each other on a local network by mapping IP addresses to MAC addresses. It also highlighted that ARP entries can change over time depending on network activity.

Task 2: Default Gateways and Routing

In this task, a more complex network was created with two subnets connected via two routers. Each subnet had two hosts connected through switches, and the routers were directly connected to form a third subnet.

IP addresses were assigned to all devices using the /etc/network/interfaces configuration file. Default gateways were configured on the hosts so that they could communicate outside their local subnet. IP forwarding was enabled on routers and disabled on hosts to ensure correct routing behavior.

After starting all nodes, the routing tables of each device were examined. It was observed that each host had a default route pointing to its respective router, while routers had routes to multiple subnets.

To test connectivity, a ping was performed from a host in one subnet to a host in another subnet. The ping was successful, confirming that the default gateways and routing configurations were working correctly.

This task demonstrated how routers and default gateways allow communication between different networks. It also emphasized the importance of proper IP addressing, routing configuration, and enabling forwarding on routers.
<img width="916" height="421" alt="net" src="https://github.com/user-attachments/assets/4465a83a-77be-4e78-85b1-1229ff9bb196" />
<img width="1006" height="553" alt="host" src="https://github.com/user-attachments/assets/f1bc03d3-22f6-45aa-b741-1a315effd0ea" />
<img width="1098" height="433" alt="host2" src="https://github.com/user-attachments/assets/5e695f4b-006f-4d69-9a45-ad5462e728a8" />
<img width="837" height="285" alt="host 3" src="https://github.com/user-attachments/assets/5b29cbcd-5cab-4dbc-a652-6d6665fb6254" />
<img width="635" height="192" alt="ping" src="https://github.com/user-attachments/assets/3e89faad-430b-46c2-81fb-ee81dfe77d64" />




