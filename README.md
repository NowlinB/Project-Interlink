# Project-Interlink
## **A collapsed core network design utilizing Cisco's Packet Tracer software**
![Project_Interlink_Topology_Full](https://github.com/NowlinB/Project-Interlink/assets/38094031/610e1c57-3300-4302-bdb3-900db980063f)
**Protocols utilized**: OSPF, SSH, EtherChannel using LACP, HSRP, NTP, FTP, VTP DNS and DHCP server configuration  

**Network security considerations** included the use of access-control lists (ACLs), dynamic arp inspection (DAI), port security, port address translation (PAT), the principle of least privilege  

Additionally, all unused ports were placed in a shutdown state   

For the convenience of any individual opening the packet tracer file to observe the configurations, passwords have not been enabled on privilege exec mode, global configuration mode, and the console line  

OSPF Area 1 makes use of a DMZ/Perimeter network to isolate the email, NTP, file and web servers   

A key focus of the project was on a redundant network design, to limit single points of failure  

Site 0 aims to simulate a simplified ISP network to allow routing exchanges between the two sites   

## Limitations  

Due to limitations of thee packet tracer software I was not able to utilize the ASA firewalls as the configuration of firewalls in packet tracer is very limited and missing many important commands    

To compensate for this i instead added routers configured to act as firewalls between the ISP and sites respectively    

Only one router module (1841) in packet tracer allows for the configuration of IPsec tunneling however this router does not support enough gigabit or fiber interfaces for a redundant network design (even with added modules)    

WLC configuration would not save after many attempts to configure, so I believe this to be a packet tracer software issue

