\# Network Architecture



\## Overview



The Enterprise SOC Lab is designed around a segmented virtual network that separates enterprise infrastructure from the attack environment. Network segmentation improves security, simplifies management, and allows attack simulations to be performed without affecting production systems.



The environment is built using VMware Workstation Pro and is protected by a pfSense firewall that manages traffic between network segments.



\---



\## Network Design



| Network | Purpose | Subnet |

|----------|---------|--------|

| VMnet2 | Corporate LAN | 10.10.10.0/24 |

| VMnet3 | WAN / External Network | 10.10.20.0/24 |



\---



\## Infrastructure



| System | Role | Planned IP Address |

|---------|------|-------------------|

| pfSense | Firewall / Router | 10.10.10.1 |

| Elastic Server | SIEM Platform | 10.10.10.10 |

| Windows Server 2022 | Domain Controller | 10.10.10.20 |

| Windows 11 Enterprise | Management Workstation | 10.10.10.30 |

| Ubuntu Server | Linux Server | 10.10.10.40 |

| Kali Linux | Attack Platform | 10.10.20.10 |



\---



\## Traffic Flow



All enterprise systems communicate through the Corporate LAN. The pfSense firewall routes and filters traffic between the internal network and the external attack network.



Centralized logging is performed by the Elastic Stack, while network traffic is monitored by Suricata IDS.



\---



\## Network Diagram



A detailed network diagram will be added after the core infrastructure has been deployed and validated.



\---



\## Design Principles



The environment was designed using the following principles:



\- Network segmentation

\- Least privilege

\- Centralized logging

\- Layered security

\- Repeatable deployment

\- Professional documentation

