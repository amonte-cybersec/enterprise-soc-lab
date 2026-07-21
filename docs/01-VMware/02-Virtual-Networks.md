\# VMware Virtual Network Configuration



\## Objective



This document describes the virtual network architecture used for the Enterprise SOC Lab environment.



The design separates the corporate environment from the attacker environment to simulate a realistic enterprise security architecture.



\---



\# Network Architecture



The lab uses VMware Workstation Pro Virtual Network Editor to create isolated host-only networks.



\---



\# Corporate Network



\## VMnet2



| Setting | Value |

|---|---|

| Network Type | Host-only |

| Network Address | 10.10.10.0/24 |

| DHCP | Disabled |

| Purpose | Enterprise internal network |



Systems planned for this network:



\- ELK SIEM

\- Windows Server Domain Controller

\- Windows 11 Employee Endpoint

\- Ubuntu Linux Server



\---



\# Attack Network



\## VMnet3



| Setting | Value |

|---|---|

| Network Type | Host-only |

| Network Address | 10.10.20.0/24 |

| DHCP | Disabled |

| Purpose | Security testing environment |



Systems planned for this network:



\- Kali Linux Attacker Machine



\---



\# Network Design



```text

VMware Workstation Pro



             |

     Virtual Network Editor



       ┌───────────────┐

       │               │

     VMnet2          VMnet3

   Corporate        Attack

 10.10.10.0/24    10.10.20.0/24



      │                │

      │                │



 ELK SIEM          Kali Linux

 Domain Controller

 Windows 11

 Ubuntu Server

```

\# Security Considerations



Network segmentation prevents attacker systems from directly existing on the same network as corporate assets.



This design allows monitoring, detection engineering, and incident response activities to be performed safely.



\---



\# Status



✅ Virtual networks created and documented.

