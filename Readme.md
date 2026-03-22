\# 🛡️ Sentinel-Node: Cyber Forensic \& Private Cloud Lab

A centralized, high-security home server architecture designed for \*\*Digital Forensic research\*\*, \*\*Network Defense\*\*, and \*\*Personal Data Sovereignty\*\*. Built as a practical implementation during my Master's in Cyber Forensic and Internet Security.


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


\## 📸 Dashboard (Mission Control)

!\[Dashboard](./dashboard.png)

\*Centralized management console via 'Homepage' showing real-time service heartbeats.\*


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



\# Launch the infrastructure

docker-compose -f docker-compose-master.yml up -d

