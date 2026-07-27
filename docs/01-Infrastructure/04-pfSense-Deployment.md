# INF-04 – pfSense Deployment

> Documents the deployment and initial configuration of pfSense for the Enterprise SOC Lab.

| Phase | Document ID | Status |
| :--- | :--- | :--- |
| Infrastructure | INF-04 | In Progress |

---

# Overview

pfSense serves as the perimeter firewall and router for the Enterprise SOC Lab. It provides the foundation for network segmentation and will eventually manage routing, firewall policies, NAT, and other network services throughout the environment.

At this stage, pfSense has been successfully installed and is accessible through the web management interface.

---

# Purpose

The pfSense firewall will provide:

- Network routing
- Firewall policy enforcement
- Network Address Translation (NAT)
- DHCP services
- DNS forwarding
- Secure separation between the WAN and LAN networks

These services will be configured during later phases of the project.

---

> [!NOTE]
> The goal of this phase was to successfully deploy pfSense and verify access to the web management interface before performing additional configuration.

---

# Deployment Summary

The following tasks have been completed:

- pfSense virtual machine created
- WAN interface connected to VMnet3
- LAN interface connected to VMnet2
- pfSense installation completed
- Initial setup wizard completed
- Web management interface accessible

Additional network configuration will be completed in future documentation.

---

# Current Network Layout

```text
                 Internet
                     │
                 VMnet3 (WAN)
                     │
               +-------------+
               |   pfSense   |
               +-------------+
                     │
                 VMnet2 (LAN)
```

---

# Validation

The following items were verified:

- pfSense boots successfully
- Interfaces assigned during installation
- WebConfigurator accessible
- Administrator login successful

---

# Screenshots

The following screenshot documents the current state of the pfSense deployment.

| Screenshot | Description |
| :--- | :--- |
| ![pfSense Dashboard](../../images/01-Infrastructure/pfsense/dashboard.png) | pfSense Dashboard after successful installation and initial login to the WebConfigurator. |

---

# Lessons Learned

- Verify interface assignments during installation.
- Use separate WAN and LAN virtual networks from the beginning.
- Confirm web interface access before configuring additional services.

---

| Previous | Phase Home | Next |
| :--- | :--- | :--- |
| [INF-03 – Virtual Networking](INF-03-Virtual-Networking.md) | [Infrastructure](README.md) | Identity Phase |