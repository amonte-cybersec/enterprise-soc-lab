\# Network Architecture



> Provides a high-level overview of the Enterprise SOC Lab network design.



\## Overview



The Enterprise SOC Lab is designed to replicate a segmented enterprise network. Traffic flows through a pfSense firewall before reaching the internal environment, allowing realistic testing of network security, monitoring, and attack simulation.



The architecture separates infrastructure into dedicated network segments to improve security, simplify management, and support future expansion.



\## Network Components



| Component | Purpose |

| :--- | :--- |

| pfSense | Firewall, routing, and NAT |

| Active Directory | Identity and authentication |

| Windows 11 Enterprise | Administrative workstation |

| Ubuntu Server | Elastic Stack |

| Kali Linux | Attack simulation |

| Suricata | Network intrusion detection |



\## Network Design



\- WAN connected through VMware NAT

\- LAN protected by pfSense

\- Internal clients joined to Active Directory

\- Centralized logging to Elastic Stack

\- Monitoring with Suricata IDS

\- Attack simulation using Kali Linux



> \*\*Note:\*\* A detailed network topology diagram will be added during the Infrastructure phase.



\## Related Documentation



\- \*\*Previous:\*\* \[Lab Objectives](02-Lab-Objectives.md)

\- \*\*Planning Home:\*\* \[Planning](README.md)

\- \*\*Next:\*\* \[Software Inventory](04-Software-Inventory.md)

