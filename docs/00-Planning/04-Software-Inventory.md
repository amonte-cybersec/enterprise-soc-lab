# PLAN-04 – Software Inventory

> Identifies the software platforms and technologies planned for the Enterprise SOC Lab.

**Phase:** Planning (00)

**Document ID:** PLAN-04

**Status:** Complete

---

## Overview

The Enterprise SOC Lab combines enterprise operating systems, security platforms, and administration tools to simulate a realistic corporate environment. The technologies selected support virtualization, identity management, monitoring, threat detection, and incident response.

## Technology Stack

### Virtualization

| Software | Purpose |
| :--- | :--- |
| VMware Workstation Pro | Hosts the virtual infrastructure |

### Operating Systems

| Software | Purpose |
| :--- | :--- |
| Windows Server 2022 | Active Directory Domain Services |
| Windows 11 Enterprise | Administrative workstation |
| Ubuntu Server | Elastic Stack host |
| Kali Linux | Attack simulation platform |

### Security & Monitoring

| Software | Purpose |
| :--- | :--- |
| pfSense CE | Firewall and routing |
| Elasticsearch | Log storage and search |
| Kibana | Security dashboards |
| Sysmon | Advanced Windows event logging |
| Winlogbeat | Windows log forwarding |
| Suricata | Network intrusion detection |

### Administration Tools

| Software | Purpose |
| :--- | :--- |
| PowerShell | Windows automation |
| Windows Admin Center *(Planned)* | Server management |
| Sysinternals Suite *(Planned)* | Windows troubleshooting |

> [!NOTE]
> ### Technology Selection
>
> The software chosen for this lab represents technologies commonly found in enterprise environments. The objective is not to use every available security product, but to understand how infrastructure, identity, networking, and monitoring platforms integrate to support security operations.

---

## Navigation

| Previous | Phase Home | Next |
| :--- | :---: | ---: |
| [← Network Architecture](03-Network-Architecture.md) | [Planning](README.md) | [PLAN-05 →](05-Project-Roadmap.md) |
