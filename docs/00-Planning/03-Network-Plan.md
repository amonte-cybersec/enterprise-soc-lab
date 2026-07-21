\# Enterprise SOC Lab - Network Plan



\## Objective



This document defines the logical network architecture used throughout the Enterprise SOC Lab.



The goal is to simulate a segmented enterprise environment where corporate assets and attacker systems operate on separate networks while remaining capable of communicating through controlled routing.



\---



\## Network Overview



The lab consists of two primary network segments:



\- Corporate Network

\- Attack Network



These networks are isolated to simulate a realistic enterprise environment while allowing controlled attack simulations.



\---



\## Network Addressing



\### Corporate Network



Network:



10.10.10.0/24



| Device | IP Address |

|----------|------------|

| ELK SIEM | 10.10.10.10 |

| Domain Controller | 10.10.10.20 |

| Windows 11 Endpoint | 10.10.10.30 |

| Ubuntu Server | 10.10.10.40 |



\---



\### Attack Network



Network:



10.10.20.0/24



| Device | IP Address |

|----------|------------|

| Kali Linux | 10.10.20.10 |



\---



\## Network Segmentation



The environment separates production resources from attacker resources to simulate enterprise security boundaries.



This allows offensive activity to be generated safely while defensive systems monitor and analyze network traffic.



\---



\## Planned Security Components



\- VMware Virtual Networks

\- pfSense Firewall

\- Suricata IDS

\- ELK SIEM



\---



\## Status



✅ Network Plan Complete



This addressing scheme will remain consistent throughout the project.

