# INF-01 - Host System

> Documents the physical workstation that hosts the Enterprise SOC Lab virtualization environment.

| Property | Value |
| :--- | :--- |
| Phase | 01 - Infrastructure |
| Document ID | INF-01 |
| Status | Complete |

---

# Overview

The Enterprise SOC Lab is hosted on a dedicated Windows workstation running VMware Workstation Pro. This system provides the compute resources required to support multiple virtual machines used throughout the lab, including pfSense, Windows Server, Windows 11, Kali Linux, and future monitoring infrastructure.

The host system serves as the foundation for every component deployed within the lab.

> [!IMPORTANT]
> A stable and properly configured host system is essential for maintaining consistent virtual machine performance and ensuring reliable lab operation.

---

# Host Information

| Component | Details |
| :--- | :--- |
| Platform | Alienware Aurora R13 |
| Operating System | Windows 11 Home |
| Processor | Intel Core i9-12900F |
| Virtualization Platform | VMware Workstation Pro |

---

# Purpose

The host system provides the physical resources required to:

- Run multiple virtual machines simultaneously.
- Support enterprise networking through VMware virtual switches.
- Host the Enterprise SOC Lab infrastructure.
- Provide a repeatable environment for security testing and documentation.

---

# Validation

The host system was verified prior to deployment by confirming:

- Windows operating system installed and fully functional.
- VMware Workstation Pro installed successfully.
- Hardware virtualization enabled.
- Sufficient processor and memory resources available for virtualization.

---

# Screenshots

| Screenshot | Description |
| :--- | :--- |
| ![System Information](../../images/01-Infrastructure/host-system/system-information.png) | Windows System Information displaying the hardware and operating system used to host the Enterprise SOC Lab. |
| ![Task Manager Performance](../../images/01-Infrastructure/host-system/task-manager-performance.png) | Task Manager Performance tab showing CPU and memory resources available for virtualization. |

---

# Lessons Learned

The host workstation forms the foundation of the Enterprise SOC Lab. Confirming hardware capabilities and virtualization support before deploying infrastructure helps prevent performance issues later in the project.

---

| Previous | Phase Home | Next |
| :--- | :---: | ---: |
| 00-Planning | 01-Infrastructure | INF-02 - VMware Workstation |