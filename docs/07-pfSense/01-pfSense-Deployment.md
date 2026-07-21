\# pfSense Deployment



\## Objective



Deploy pfSense Community Edition as the perimeter firewall for the Enterprise SOC Lab.



\---



\## Purpose



The pfSense firewall provides:



\- Network segmentation

\- Routing between security zones

\- Firewall policy enforcement

\- DNS Resolver services

\- Enterprise perimeter security



\---



\## Virtual Machine Configuration



| Setting | Value |

|---------|-------|

| Name | pfSense-Firewall |

| Operating System | FreeBSD 64-bit |

| vCPU | 1 |

| Memory | 1 GB |

| Disk | 20 GB |

| Network Adapter 1 | WAN |

| Network Adapter 2 | LAN |



\---



\## Network Design



| Interface | VMware Network | Purpose |

|-----------|----------------|---------|

| WAN | VMnet3 (After Installation) | Attack / External Network |

| LAN | VMnet2 | Corporate Network |



\---



\## Installation Notes



During installation, the WAN interface was temporarily connected to \*\*VMware NAT (VMnet8)\*\*.



This allowed the Netgate Installer to reach the Netgate update servers and complete the installation successfully.



After installation, the WAN interface will be changed back to \*\*VMnet3\*\* to match the Enterprise SOC Lab network architecture.



\---



\## Lessons Learned



The Netgate Installer requires temporary Internet connectivity during deployment.



Using VMware NAT for the WAN interface allows the installer to complete successfully before transitioning to an isolated enterprise lab network.



\---



\## Status



\- ✅ pfSense VM Created

\- ✅ pfSense Installed

\- ✅ Interface Assignment Verified

\- ⏳ WAN Interface Pending Migration to VMnet3

