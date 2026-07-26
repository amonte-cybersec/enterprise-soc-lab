# Infrastructure

> Documents the deployment of the virtual infrastructure that powers the Enterprise SOC Lab.

**Phase:** Infrastructure (01)

**Status:** In Progress

---

## Overview

The Infrastructure phase focuses on building the foundation of the Enterprise SOC Lab. This includes preparing the host system, configuring VMware Workstation Pro, deploying virtual networking, installing pfSense, and validating connectivity between all virtual machines.

The completed infrastructure provides a stable platform for identity services, security monitoring, attack simulation, and incident response activities documented in later phases.

---

## Documentation

| Document ID | Title | Description |
| :--- | :--- | :--- |
| INF-01 | [Host System](01-Host-System.md) | Documents the physical workstation used to host the lab environment. |
| INF-02 | [VMware Workstation](02-VMware-Workstation.md) | Covers the installation and configuration of VMware Workstation Pro. |
| INF-03 | [Virtual Networks](03-Virtual-Networks.md) | Documents the isolated virtual networks used throughout the lab. |
| INF-04 | [pfSense Deployment](04-pfSense-Deployment.md) | Describes the deployment and initial configuration of the pfSense firewall. |
| INF-05 | [Management Workstation](05-Management-Workstation.md) | Documents the Windows management virtual machine used to administer the environment. |
| INF-06 | [Network Validation](06-Network-Validation.md) | Verifies connectivity and communication throughout the virtual environment. |
| INF-07 | [Troubleshooting](07-Troubleshooting.md) | Documents deployment challenges, resolutions, and lessons learned. |

---

## Phase Deliverables

Upon completion of this phase, the following objectives will be achieved:

- Dedicated virtualization platform configured
- Isolated virtual networking deployed
- pfSense firewall operational
- Windows management workstation deployed
- Network connectivity validated
- Deployment documentation completed

> [!IMPORTANT]
> ### Build a Stable Foundation
>
> Every enterprise environment depends on reliable infrastructure. Completing and validating the virtualization platform before deploying additional services reduces complexity and creates a consistent baseline for future configuration and troubleshooting.

---

## Navigation

| Previous Phase | Repository Home | Next Document |
| :--- | :---: | ---: |
| [← Planning](../00-Planning/README.md) | [Enterprise SOC Lab](../../README.md) | [Host System →](01-Host-System.md) |