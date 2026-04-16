Week 05 Tutorial Report – COIT20261

In this week’s tutorial, I learned about VLANs and how they are used to separate networks logically even when devices are connected to the same physical switch.

In the first task, I created a GNS3 project with four Linux hosts and an OpenvSwitch. Initially, I configured all hosts in the same subnet and verified that they could communicate with each other using ping. After that, I set up VLANs on the switch by assigning different VLAN IDs to specific ports. Two hosts were placed in one VLAN and the other two in a different VLAN. Once the VLANs were configured, I tested connectivity again and noticed that hosts in different VLANs could no longer communicate with each other. This helped me understand how VLANs isolate network traffic even within the same physical network. I also checked ARP tables to observe how devices were resolving addresses within their VLAN.

In the second task, I extended the setup by adding a Linux router to enable communication between the VLANs. I configured the switch port connected to the router as a trunk port so it could carry traffic from multiple VLANs. On the router side, I created sub-interfaces for each VLAN and assigned IP addresses to them. This allowed the router to act as a gateway for both VLANs. After completing the configuration, I tested connectivity again and confirmed that all hosts could now communicate with each other across VLANs.

Overall, this tutorial helped me clearly understand the difference between access ports and trunk ports, how VLANs work in practice, and how routing between VLANs is achieved using a router. It also gave me hands-on experience with OpenvSwitch and Linux networking commands.
<img width="1884" height="772" alt="1" src="https://github.com/user-attachments/assets/e715b24e-2df4-4d13-9892-8224c9266ebc" />
<img width="1019" height="513" alt="2" src="https://github.com/user-attachments/assets/9a97ce4e-733f-4221-8a90-f0a6b0a5dc86" />
<img width="1087" height="470" alt="3" src="https://github.com/user-attachments/assets/51efa243-cca3-4055-87f4-6dada2874400" />
<img width="880" height="935" alt="4" src="https://github.com/user-attachments/assets/43e5fd1c-9f7e-4181-ad54-77df36b9ca2c" />
<img width="613" height="477" alt="4-1" src="https://github.com/user-attachments/assets/701ae287-7714-4370-814d-dac4834f9a7a" />
<img width="882" height="636" alt="5" src="https://github.com/user-attachments/assets/dce25f2e-1f6b-472e-88b5-11b22568835b" />
<img width="929" height="555" alt="6" src="https://github.com/user-attachments/assets/8c589e06-b6da-441c-872a-4128ebfea0e9" />
<img width="1396" height="868" alt="7" src="https://github.com/user-attachments/assets/96abded1-25d6-4abf-a50e-b0b79d7642c0" />
<img width="782" height="526" alt="8" src="https://github.com/user-attachments/assets/952ed31b-4f98-4e63-a046-6dc61a626ea2" />

