# VMware Workstation

> Documents the installation and configuration of VMware Workstation Pro used to host the Enterprise SOC Lab.

**Phase:** Infrastructure (01)

**Document ID:** INF-02

**Status:** Complete

---

## Overview

VMware Workstation Pro serves as the primary virtualization platform for the Enterprise SOC Lab. It provides the ability to create, manage, and isolate multiple virtual machines while supporting custom virtual networking required for enterprise infrastructure simulations.

The platform enables the deployment of Windows, Linux, and network appliance virtual machines that form the foundation of the lab environment.

---

## Software Information

| Component | Configuration |
| :--- | :--- |
| Software | VMware Workstation Pro |
| Purpose | Desktop Virtualization Platform |
| Host Operating System | Windows 11 Home |
| Hypervisor Type | Type-2 Hypervisor |
| Deployment Status | Installed and Operational |

---

## Why VMware Workstation?

VMware Workstation Pro was selected because it provides enterprise-grade virtualization features, including custom virtual networking, virtual machine snapshots, hardware customization, and support for multiple operating systems.

These capabilities allow the lab to closely simulate an enterprise infrastructure while remaining portable and easy to manage.

---

## Configuration Summary

| Setting | Value |
| :--- | :--- |
| Virtualization Support | Enabled |
| Custom VM Networks | Configured |
| Snapshot Support | Enabled |
| Multiple Concurrent VMs | Supported |

---

## Screenshots

| Screenshot | Description |
| :--- | :--- |
| ![VMware Home](../../images/01-Infrastructure/vmware/vmware-home.png) | VMware Workstation Pro home interface after installation. |
| ![VMware Version](../../images/01-Infrastructure/vmware/vmware-version.png) | Installed VMware Workstation Pro version information. |
| ![Virtual Network Editor](../../images/01-Infrastructure/vmware/virtual-network-editor.png) | VMware Virtual Network Editor showing configured virtual networks. |

> [!TIP]
> ### Best Practice
>
> Configure virtual networking before deploying virtual machines. Establishing VMnet assignments early prevents unnecessary reconfiguration and helps maintain a consistent network design throughout the project.

---

## Validation

The VMware installation was validated by confirming:

- VMware Workstation Pro launches successfully.
- Virtual machines can be created and powered on.
- Custom virtual networks are available.
- Hardware virtualization is functioning correctly.
- Snapshot functionality is operational.

---

## Lessons Learned

A properly configured virtualization platform simplifies every deployment that follows. Spending time validating VMware settings before creating virtual machines reduces deployment issues and provides a stable foundation for the entire lab.

---

## Navigation

| Previous | Phase Home | Next |
| :--- | :---: | ---: |
| [← Host System](01-Host-System.md) | **Infrastructure** | [Virtual Networks →](03-Virtual-Networks.md) |