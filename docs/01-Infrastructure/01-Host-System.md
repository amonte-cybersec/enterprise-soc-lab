# Host System

> Documents the physical workstation that hosts the Enterprise SOC Lab virtual environment.

**Phase:** Infrastructure (01)

**Document ID:** INF-01

**Status:** Complete

---

## Overview

The Enterprise SOC Lab is hosted on a dedicated Windows workstation capable of supporting multiple virtual machines simultaneously. The host system provides the processing power, memory, and storage required to run enterprise infrastructure components including Active Directory, pfSense, ELK, Windows Server, Windows 11, Ubuntu Server, and Kali Linux.

Selecting capable hardware ensures the lab remains responsive while accurately simulating an enterprise environment.

---

## Host Specifications

| Component | Configuration |
| :--- | :--- |
| Host System | Alienware Aurora R13 |
| Processor | Intel Core i9-12900F |
| Operating System | Windows 11 Home (64-bit) |
| Hypervisor | VMware Workstation Pro |
| Virtualization | Intel VT-x Enabled |
| Primary Purpose | Enterprise SOC Lab Host |

---

## Hardware Considerations

The host workstation was selected to provide sufficient computing resources for running multiple virtual machines concurrently. Enterprise security environments frequently require several systems to operate simultaneously, making processor performance, available memory, and storage capacity critical factors when designing the lab.

The virtualization platform allows isolated systems to communicate across dedicated virtual networks while remaining independent of the physical host operating system.

---

## Environment

| Component | Value |
| :--- | :--- |
| Hypervisor | VMware Workstation Pro |
| Host Operating System | Windows 11 Home |
| Virtualization Platform | Type-2 Hypervisor |
| Lab Purpose | Enterprise Security Operations Center |

---

## Validation

The host environment was validated by confirming:

- VMware Workstation Pro launches successfully.
- Hardware virtualization is enabled.
- Virtual machines power on without hardware errors.
- Multiple virtual machines can operate simultaneously.
- Host operating system remains stable during lab operation.

> [!NOTE]
> ### Engineering Insight
>
> Enterprise virtualization begins with reliable hardware. A stable host platform reduces resource bottlenecks, improves virtual machine performance, and provides a dependable foundation for every service deployed throughout the lab.

---

## Lessons Learned

Enterprise environments rely on a stable infrastructure layer before additional services are introduced. Verifying host hardware, virtualization support, and hypervisor functionality early helps eliminate issues that could impact later deployment phases.

---

## Navigation

| Previous | Phase Home | Next |
| :--- | :---: | ---: |
| [← Infrastructure](README.md) | **Infrastructure** | [VMware Workstation →](02-VMware-Workstation.md) |