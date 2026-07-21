\# VMware Resource Plan



\## Objective



This document defines the virtual machine resource allocation used throughout the Enterprise SOC Lab.



The goal is to create a realistic enterprise security environment while maintaining efficient resource usage on the host system.



\---



\# Host Resource Considerations



The lab is hosted on:



\- Alienware Aurora R13

\- Intel Core i9-12900F Processor

\- 16 CPU Cores / 24 Logical Processors

\- 32 GB RAM

\- 614 GB Available Storage



Resource allocation is designed to balance performance between the virtual environment and the host operating system.



\---



\# Virtual Machine Resource Allocation



| Virtual Machine | Operating System | Role | vCPU | RAM | Storage |

|---|---|---|---|---|---|

| ELK SIEM | Ubuntu Server | Log collection, analysis, and dashboards | 4 | 6 GB | 80 GB |

| Domain Controller | Windows Server | Active Directory, DNS, authentication | 2 | 3 GB | 60 GB |

| Employee Workstation | Windows 11 | Corporate endpoint simulation | 2 | 4 GB | 64 GB |

| Linux Server | Ubuntu Server | Internal enterprise Linux system | 2 | 2 GB | 40 GB |

| Kali Linux | Kali Linux | Attack simulation environment | 2 | 3 GB | 50 GB |

| pfSense Firewall | FreeBSD | Network segmentation and routing | 1 | 1 GB | 20 GB |



\---



\# Total Planned Resource Usage



\## Memory Allocation



| Resource | Amount |

|---|---:|

| Total Lab RAM Usage | 19 GB |

| Host Available RAM | 13 GB |



\---



\## CPU Allocation



| Resource | Amount |

|---|---:|

| Allocated Virtual CPUs | 13 vCPU |

| Host Processor | 16 Cores / 24 Logical Processors |



\---



\## Storage Allocation



| Resource | Amount |

|---|---:|

| Planned Virtual Storage | \~314 GB |

| Available Host Storage | 614 GB |



\---



\# Storage Configuration



Virtual disks will use thin provisioning.



This allows VMware to allocate storage dynamically as virtual machines require additional space rather than immediately consuming the maximum configured disk size.



\---



\# Resource Management Strategy



The Enterprise SOC Lab intentionally avoids maximum resource allocation.



Resources are limited to simulate realistic enterprise constraints while maintaining host system stability.



Virtual machine performance will be monitored and adjusted during deployment.



\---



\# Status



✅ Resource planning completed



Next phase:



\- Install VMware Workstation Pro

\- Configure virtual networks

\- Begin virtual machine deployment

