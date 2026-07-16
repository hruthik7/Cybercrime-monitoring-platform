# Cybercrime-monitoring-platform
“A security lab environment focused on SIEM deployment, behavioral threat hunting, and vulnerability management using Wazuh and Docker.”
# Cybercrime Detection and Monitoring Lab

## Executive Summary
This project demonstrates the deployment and management of a professional-grade SIEM (Security Information and Event Management) environment. The lab was designed to practice real-world threat hunting, system auditing, and vulnerability management.

## Technical Architecture
* **Host System:** Windows 11
* **Virtualization:** Docker Desktop, WSL 2 (Ubuntu)
* **Security Stack:** Wazuh (Manager, Indexer, Dashboard, Agent)

## Project Methodology
### Phase 1: Environment & Infrastructure
* Established WSL 2 environment for Linux container hosting.
* Optimized Docker configuration (Disabled "Resource Saver" mode) to ensure persistent bridge connectivity.

### Phase 2: Deployment
* Orchestrated multi-service architecture using `docker-compose`.
* Successfully integrated host endpoint (`HV_679`) for real-time telemetry.

### Phase 3: Threat Hunting & Remediation
* **Vulnerability Management:** Detected and remediated critical Git vulnerability (CVE-2024-32002) using `winget`.
* **File Integrity Monitoring:** Validated system auditing capabilities by triggering and detecting unauthorized file changes.

## Engineering Resilience
During deployment, I resolved complex networking issues between the Windows host and WSL 2. This process of debugging and bridge engineering was critical in achieving a stable, persistent security monitoring environment.

## Getting Started

### Prerequisites
- **OS:** Windows 10/11 with WSL 2 (Ubuntu) enabled.
- **Containerization:** Docker Desktop installed and running with "WSL 2 Integration" enabled.

### Deployment Instructions
To replicate this lab environment locally:

 **Clone the repository:**
   ```bash
   git clone [https://github.com/hruthik7/Cybercrime-monitoring-platform](https://github.com/hruthik7/Cybercrime-monitoring-platform)
   cd Cybercrime-monitoring-platform
---
*Created as a proactive defense research project.*
