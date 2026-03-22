\# 🛡️ Sentinel-Node: Cyber Forensic \& Private Cloud Lab



\[!\[Docker](https://img.shields.io/badge/Docker-24.0.5-blue?logo=docker)](https://www.docker.com/)

\[!\[License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

\[!\[Uptime](https://img.shields.io/badge/Uptime-99.9%25-brightgreen)](https://github.com/yourusername/Sentinel-Node)



A centralized, high-security home server architecture designed for \*\*Digital Forensic research\*\*, \*\*Network Defense\*\*, and \*\*Personal Data Sovereignty\*\*. Built as a practical implementation during my Master's in Cyber Forensic and Internet Security.



\---



\## 🏗️ System Architecture

Sentinel-Node transforms a standard Intel i5/i7 hardware stack into a "Digital Vault" using a modular Docker-compose orchestration. 



\### 🔍 Cyber Forensic Lab

\* \*\*FileBrowser:\*\* Remote management and ingestion of evidence for the 1TB Seagate HDD array.

\* \*\*Stirling-PDF:\*\* Privacy-first, locally-hosted PDF toolkit for forensic report sanitization.

\* \*\*Vaultwarden:\*\* Bitwarden-compatible server for encrypted investigation credential management.



\### 🛡️ Network \& Infrastructure

\* \*\*AdGuard Home:\*\* Network-wide DNS sinkhole for malware blocking and forensic traffic analysis.

\* \*\*Scrutiny:\*\* Low-level S.M.A.R.T. monitoring and thermal auditing of physical storage media (/dev/sda).

\* \*\*Netdata:\*\* Real-time, per-second kernel-level performance monitoring.

\* \*\*Watchtower:\*\* Automated container lifecycle management and security patching.



\---



\## 📸 Dashboard (Mission Control)

!\[Dashboard](./dashboard.png)

\*Centralized management console via 'Homepage' showing real-time service heartbeats.\*



\---



\## 📂 Project Structure

```text

Sentinel-Node/

├── README.md

├── docker-compose-master.yml    # Master Template (Sanitized)

├── .gitignore                  # Forensic Safety Filters

└── services/                   # Service Configuration Files

&#x20;   ├── adguard/                # DNS Security Config

&#x20;   ├── vaultwarden/            # Encrypted Vault Data

&#x20;   ├── scrutiny/               # HDD Health Metrics

&#x20;   └── homepage/               # Dashboard Layouts



🚀 Deployment \& Maintenance

This lab is designed for "Set and Forget" operational security.



1\. Requirements

Docker \& Docker Compose



Tailscale (for Zero-Trust Remote Access)



Intel i5/i7 Processor with VT-x enabled



2\. Quick Start

Bash

\# Clone the repository

git clone \[https://github.com/yourusername/Sentinel-Node.git](https://github.com/yourusername/Sentinel-Node.git)

cd Sentinel-Node



\# Launch the infrastructure

docker-compose -f docker-compose-master.yml up -d

