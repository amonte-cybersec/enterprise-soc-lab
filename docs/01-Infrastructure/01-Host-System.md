# INF-01 - Host System

> Documents the physical workstation that hosts the Enterprise SOC Lab virtualization environment.

| Property | Value |
| :--- | :--- |
| **Phase** | 01 - Infrastructure |
| **Document ID** | INF-01 |
| **Status** | Complete |

---

# Overview

The Enterprise SOC Lab is hosted on a dedicated Windows workstation running VMware Workstation Pro. This workstation provides the processing power and virtualization capabilities required to build a realistic enterprise environment for security operations, system administration, and incident response.

The host system serves as the foundation for every virtual machine deployed throughout the project.

> [!IMPORTANT]
> Every component within the Enterprise SOC Lab depends on the stability and performance of the host system. Verifying the host environment before deploying infrastructure reduces troubleshooting later in the project.

---

# Scope

This document covers:

- Physical host hardware
- Host operating system
- Virtualization platform
- Initial validation

Additional infrastructure components such as VMware networking and pfSense are documented separately.

---

# Host Information

| Component | Details |
| :--- | :--- |
| Computer | Alienware Aurora R13 |
| Operating System | Windows 11 Home |
| Processor | Intel Core i9-12900F |
| Hypervisor | VMware Workstation Pro |

---

# Purpose

The host workstation provides the physical resources required to:

- Host enterprise virtual machines
- Support multiple operating systems simultaneously
- Run VMware Workstation Pro
- Provide a repeatable cybersecurity lab environment
- Support future Active Directory and SOC infrastructure

> [!TIP]
> Building on dedicated hardware creates a consistent environment for testing, documentation, and future expansion.

---

# Validation

The host environment was validated by confirming:

- Windows operating system installed successfully.
- VMware Workstation Pro launches correctly.
- Hardware virtualization is enabled.
- System resources are available for virtualization.

---

# Evidence

## Screenshots

| Screenshot | Description |
| :--- | :--- |
| ![System Information](../../images/01-Infrastructure/host-system/system-information.png) | Windows System Information displaying the hardware and operating system used to host the Enterprise SOC Lab. |
| ![Task Manager Performance](../../images/01-Infrastructure/host-system/task-manager-performance.png) | Task Manager Performance showing available CPU and memory resources for virtualization workloads. |

> [!NOTE]
> Screenshots are captured immediately after successful validation to accurately document the current state of the environment.

---

# Lessons Learned

Establishing a stable host platform before deploying virtual infrastructure creates a reliable foundation for the remainder of the Enterprise SOC Lab. Early validation minimizes deployment issues during future phases.

---

# Related Documentation

- [Infrastructure README](README.md)
- [INF-02 - VMware Workstation](INF-02-VMware-Workstation.md)

---

## Navigation

⬅️ **Previous:** [Planning README](../00-Planning/README.md)

🏠 **Phase Home:** [Infrastructure README](README.md)

➡️ **Next:** [INF-02 - VMware Workstation](INF-02-VMware-Workstation.md)