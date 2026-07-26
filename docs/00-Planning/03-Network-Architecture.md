# Network Architecture

> Provides a high-level overview of the Enterprise SOC Lab network design.

**Phase:** Planning (00)

**Document ID:** PLAN-03

**Status:** Complete

---

## Overview

The Enterprise SOC Lab is designed around a segmented network architecture that reflects common enterprise environments. The lab separates management, infrastructure, monitoring, and attack simulation into dedicated virtual machines connected through a centralized firewall.

This design supports secure administration, centralized logging, realistic attack scenarios, and scalable expansion throughout future project phases.

## Architecture Components

| Component | Role |
| :--- | :--- |
| VMware Workstation Pro | Hosts the virtual infrastructure |
| pfSense CE | Firewall, routing, and NAT |
| Windows Server 2022 | Active Directory Domain Services |
| Windows 11 Enterprise | Administrative workstation |
| Ubuntu Server | Elastic Stack (Elasticsearch & Kibana) |
| Kali Linux | Attack simulation platform |

## Network Design Principles

- Segmented virtual networks
- Centralized firewall management
- Secure administrative access
- Centralized log collection
- Enterprise identity management
- Expandable infrastructure for future phases

> [!IMPORTANT]
> ### Why Architecture Matters
>
> Designing the environment before deployment establishes clear system roles, communication paths, and security boundaries. A well-planned architecture simplifies expansion, improves troubleshooting, and reduces unnecessary configuration changes later in the project.

---

## Navigation

| Previous | Phase Home | Next |
| :--- | :---: | ---: |
| [← Lab Objectives](02-Lab-Objectives.md) | [Planning](README.md) | [Software Inventory →](04-Software-Inventory.md) |
