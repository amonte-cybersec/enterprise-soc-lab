# INF-03 - Virtual Networks

> Documents the virtual networking architecture used to provide network segmentation for the Enterprise SOC Lab.

| Property | Value |
| :--- | :--- |
| Phase | 01 - Infrastructure |
| Document ID | INF-03 |
| Status | Complete |

---

# Overview

The Enterprise SOC Lab uses VMware Workstation's Virtual Network Editor to create isolated network segments. These networks simulate a basic enterprise environment by separating internal systems from external connectivity.

The lab currently consists of two custom virtual networks that will be used throughout the project.

> [!IMPORTANT]
> Network segmentation is a fundamental security practice. Separating internal and external traffic creates a more realistic enterprise environment and provides a foundation for future firewall and monitoring configurations.

---

# Virtual Network Configuration

| Network | Purpose |
| :--- | :--- |
| VMnet2 | Internal Corporate LAN |
| VMnet3 | External / WAN Network |

---

# Purpose

The virtual networking environment provides the ability to:

- Isolate enterprise systems from the host network.
- Simulate internal and external network segments.
- Support pfSense as the network gateway.
- Create a realistic environment for future monitoring and attack simulations.

---

# Configuration Summary

The virtual networking environment has been prepared with:

- Custom VMnet2 network created.
- Custom VMnet3 network created.
- Networks available for virtual machine assignment.
- Network segmentation established for future infrastructure deployment.

---

# Validation

The virtual networking configuration was validated by confirming:

- VMnet2 is available within VMware Workstation.
- VMnet3 is available within VMware Workstation.
- Both networks can be assigned to virtual machines.
- Virtual Network Editor reflects the intended lab topology.

---

# Screenshots

| Screenshot | Description |
| :--- | :--- |
| ![VMnet2 Configuration](../../images/01-Infrastructure/networking/vmnet2-config.png) | VMware Virtual Network Editor showing the configuration of VMnet2 for the internal corporate network. |
| ![VMnet3 Configuration](../../images/01-Infrastructure/networking/vmnet3-config.png) | VMware Virtual Network Editor showing the configuration of VMnet3 for the external/WAN network. |

---

# Lessons Learned

Creating dedicated virtual networks before deploying servers and workstations establishes a structured foundation for the lab. Proper network segmentation simplifies future firewall configuration, Active Directory deployment, and security monitoring.

---

| Previous | Phase Home | Next |
| :--- | :---: | ---: |
| INF-02 - VMware Workstation | 01-Infrastructure | INF-04 - pfSense Deployment |