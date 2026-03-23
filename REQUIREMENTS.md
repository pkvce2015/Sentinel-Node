# 📋 System Requirements: Sentinel-Node Lab

This document outlines the hardware and software specifications required to deploy and maintain the Sentinel-Node Forensic Lab environment.

## 💻 Hardware Specifications (Minimum)
To ensure stable performance during forensic imaging and concurrent container operations, the following specs are recommended:

* **Processor:** Intel Core i5 (6th Gen) or higher (VT-x/AMD-V support required for virtualization).
* **Memory:** 8GB RAM (16GB+ recommended for Immich machine learning and Nextcloud AIO).
* **Primary Storage:** 128GB SSD (Boot drive & Docker volumes).
* **Forensic Storage:** 1TB+ HDD (Dedicated for evidence storage and media backups).
* **Network:** Gigabit Ethernet or stable Wi-Fi with Static IP or Tailscale configuration.

## 🐧 Software Environment
The lab is optimized for Linux-based environments but can be managed from any workstation.

* **Host OS:** Ubuntu 24.04 LTS (Recommended) or any Debian-based distribution.
* **Docker Engine:** Version 24.x or higher.
* **Docker Compose:** Version 2.x or higher.
* **File System:** EXT4 or ZFS (for data integrity and snapshot capabilities).

## 🛡️ Network & Access Requirements
* **Tailscale:** Required for secure, Zero-Trust remote access without opening router ports.
* **Port Availability:** * `53/udp`: AdGuard Home (DNS)
    * `80/443`: Web Traffic
    * `3000`: Homepage Dashboard
    * `8080-8084`: Individual Service UIs

## 🔧 Kernel Dependencies
For hardware monitoring (Scrutiny) to function correctly, the host must support:
* **S.M.A.R.T. Tools:** `smartmontools` installed on the host.
* **Thermal Monitoring:** `drivetemp` or `lm-sensors` kernel modules loaded.
