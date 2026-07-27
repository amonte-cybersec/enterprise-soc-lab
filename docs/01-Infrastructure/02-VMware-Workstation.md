# INF-02 - VMware Workstation

> Documents the installation and configuration of VMware Workstation Pro, which provides the virtualization platform for the Enterprise SOC Lab.

| Property | Value |
| :--- | :--- |
| Phase | 01 - Infrastructure |
| Document ID | INF-02 |
| Status | Complete |

---

# Overview

VMware Workstation Pro was selected as the hypervisor for the Enterprise SOC Lab due to its enterprise-grade virtualization capabilities, custom networking options, and support for multiple operating systems.

All virtual machines used throughout this project are deployed and managed through VMware Workstation Pro.

> [!NOTE]
> VMware Workstation serves as the virtualization layer between the physical host system and all virtual infrastructure deployed within the lab.

---

# Software Information

| Component | Details |
| :--- | :--- |
| Hypervisor | VMware Workstation Pro |
| Host Operating System | Windows 11 Home |
| Installation Status | Installed |
| Virtualization | Intel VT-x Enabled |

---

# Purpose

VMware Workstation provides the virtualization platform required to:

- Create isolated enterprise virtual machines.
- Support multiple operating systems simultaneously.
- Configure custom virtual networking.
- Simulate a production enterprise environment.
- Snapshot and restore lab environments when necessary.

---

# Configuration Summary

The VMware environment has been prepared with:

- VMware Workstation Pro installed.
- Virtualization support verified.
- Enterprise SOC Lab workspace created.
- Custom virtual networking configured for future infrastructure deployment.

---

# Validation

The installation was validated by confirming:

- VMware Workstation launches successfully.
- Virtual machines can be created.
- Virtual Network Editor is accessible.
- Custom VMnet networks are available.

---

# Screenshots

| Screenshot | Description |
| :--- | :--- |
| ![VMware Home](../../images/01-Infrastructure/vmware/vmware-home.png) | VMware Workstation Pro showing the Enterprise SOC Lab virtual machine inventory. |
| ![VMware Version](../../images/01-Infrastructure/vmware/vmware-version.png) | Installed VMware Workstation Pro version information. |
| ![Virtual Network Editor](../../images/01-Infrastructure/vmware/virtual-network-editor.png) | Virtual Network Editor displaying the custom VMnet2 and VMnet3 configurations. |

---

# Lessons Learned

Deploying VMware Workstation before building the lab establishes a consistent virtualization platform and simplifies future infrastructure deployment. Verifying installation and networking early reduces troubleshooting during later phases.

---

| Previous | Phase Home | Next |
| :--- | :---: | ---: |
| INF-01 - Host System | 01-Infrastructure | INF-03 - Virtual Networks |