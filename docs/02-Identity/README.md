# Identity

> Deploy and configure the Windows identity infrastructure that supports authentication, authorization, and centralized administration throughout the Enterprise SOC Lab.

| Phase | Status |
| :--- | :--- |
| Identity | In Progress |

---

# Overview

The Identity phase establishes the Windows infrastructure required to manage users, devices, and security policies within the Enterprise SOC Lab. This includes deploying a dedicated management workstation, configuring Windows Server, implementing Active Directory Domain Services (AD DS), and preparing client systems for domain integration.

Completing this phase provides the centralized identity platform used by the remaining monitoring, detection, and incident response components of the lab.

> [!IMPORTANT]
> ### Build Identity Before Security
>
> Most enterprise security solutions rely on a properly configured identity infrastructure. Establishing Active Directory, DNS, and centralized administration before deploying security tools creates a stable foundation that simplifies management and improves visibility across the environment.

---

# Objectives

- Deploy a Windows 11 management workstation
- Install and configure Windows Server
- Deploy Active Directory Domain Services
- Configure DNS and DHCP
- Create Organizational Units (OUs)
- Create users, groups, and service accounts
- Configure baseline Group Policy Objects (GPOs)
- Join client systems to the domain

---

# Documents

| ID | Document | Status |
| :--- | :--- | :--- |
| ID-01 | [Management Workstation](ID-01-Management-Workstation.md) | Complete |
| ID-02 | [Windows Server](ID-02-Windows-Server.md) | Not Started |
| ID-03 | [Active Directory](ID-03-Active-Directory.md) | Not Started |
| ID-04 | [DNS](ID-04-DNS.md) | Not Started |
| ID-05 | [DHCP](ID-05-DHCP.md) | Not Started |
| ID-06 | [Organizational Units](ID-06-Organizational-Units.md) | Not Started |
| ID-07 | [Groups and Users](ID-07-Groups-and-Users.md) | Not Started |
| ID-08 | [Group Policy](ID-08-Group-Policy.md) | Not Started |
| ID-09 | [Domain-Joined Client](ID-09-Domain-Joined-Client.md) | Not Started |

---

# Phase Deliverables

- Windows 11 Management Workstation
- Windows Server 2022
- Active Directory Domain Services
- DNS Infrastructure
- DHCP Services
- Organizational Unit Structure
- Enterprise User and Group Management
- Baseline Group Policy Configuration
- Domain-Joined Windows Client

---

# Navigation

| Previous | Phase Home | Next |
| :--- | :--- | :--- |
| [Infrastructure](../01-Infrastructure/README.md) | Identity | [ID-01](ID-01-Management-Workstation.md) |