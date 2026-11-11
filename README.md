# NetScope
### Cloud-Based Network Security, Monitoring & Diagnostics Platform

NetScope is a network monitoring and diagnostics platform designed to provide visibility into network activity, automate connectivity analysis, identify exposed services, and monitor infrastructure health. It combines network discovery, packet analysis, automated diagnostics, and cloud infrastructure monitoring into a centralised platform.

The project explores the integration of Linux networking utilities, Python-based automation, network analysis tools, and AWS cloud services to build a practical network observability and security solution.

**Status:** 🚧 In Development

---

## Overview

Modern network infrastructures require continuous monitoring, efficient troubleshooting, and visibility into network activity. Diagnosing connectivity issues, identifying exposed services, and understanding traffic behaviour often involve multiple independent tools.

NetScope aims to bring these capabilities together through an automated monitoring and diagnostics platform.

The system is designed to collect network information, execute diagnostic operations, analyse traffic patterns, and present actionable insights through a centralised dashboard.

## Key Objectives

- **Network Discovery:** Identify reachable hosts, open ports, and exposed network services.
- **Connectivity Monitoring:** Monitor host availability, response times, and network reachability.
- **Packet Analysis:** Capture and inspect network traffic to understand communication patterns and protocol behaviour.
- **Automated Diagnostics:** Automate common network troubleshooting operations using Python and Shell scripting.
- **Security Visibility:** Identify potentially suspicious network activity and unusual connection patterns.
- **Cloud Infrastructure Monitoring:** Explore cloud deployment, infrastructure isolation, and resource monitoring using AWS.
- **Centralised Visualisation:** Present network statistics, diagnostic results, and monitoring information through an interactive dashboard.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming | Python |
| Scripting | Bash / Shell |
| Operating System | Linux |
| Network Discovery | Nmap |
| Packet Capture | TCPDump |
| Packet Analysis | Wireshark |
| Backend | FastAPI |
| Frontend | React, Tailwind CSS |
| Cloud Platform | Amazon Web Services (AWS) |
| Compute | Amazon EC2 |
| Cloud Networking | VPC, Security Groups |
| Monitoring | Amazon CloudWatch |
| Storage | Amazon S3 |

## System Architecture

NetScope follows a modular architecture consisting of network collection, diagnostic processing, analysis, cloud infrastructure, and visualisation layers.

```text
                 NETWORK ENVIRONMENT
                         |
             +-----------+-----------+
             |                       |
        Network Scanning       Packet Capture
             |                       |
           Nmap                  TCPDump
             |                       |
             +-----------+-----------+
                         |
               DATA COLLECTION LAYER
                         |
                 ANALYSIS ENGINE
                         |
                 Python / Bash
                         |
             +-----------+-----------+
             |                       |
       Network Diagnostics      Traffic Analysis
             |                       |
             +-----------+-----------+
                         |
                  FASTAPI BACKEND
                         |
                  REST API LAYER
                         |
                 REACT DASHBOARD
                         |
               VISUALISATION LAYER
                         |
                 AWS INFRASTRUCTURE
                         |
              EC2 | VPC | S3 | CloudWatch
```

## Core Modules

### 1. Network Discovery & Scanning
Uses Nmap to discover hosts, identify open ports, and inspect running services across authorised network environments.

### 2. Network Diagnostics
Uses Python, Bash, and Linux networking utilities to automate connectivity checks, DNS resolution, host availability monitoring, and network troubleshooting.

### 3. Packet Capture & Traffic Analysis
Uses TCPDump for packet capture and Wireshark for protocol inspection and traffic analysis. Captured traffic can be examined to understand communication patterns and identify relevant network events.

### 4. Network Monitoring & Visualisation
Provides a centralised dashboard for displaying network availability, discovered hosts, open ports, response times, traffic statistics, and diagnostic reports.

### 5. Cloud Infrastructure & Monitoring
Explores AWS-based deployment and infrastructure monitoring using:

- **EC2:** Application hosting and compute infrastructure.
- **VPC:** Isolated cloud networking environment.
- **Security Groups:** Network traffic access control.
- **S3:** Storage for diagnostic reports and captured data.
- **CloudWatch:** Infrastructure metrics, logs, and monitoring.

## Project Structure

```text
NetScope/
│
├── backend/
│   ├── app/
│   │   ├── api/
│   │   ├── services/
│   │   ├── utils/
│   │   └── main.py
│   │
│   └── requirements.txt
│
├── frontend/
│
├── scripts/
│
├── captures/
│
├── reports/
│
├── docs/
│
├── README.md
└── .gitignore
```

## Development Roadmap

- [ ] Establish project architecture and development environment.
- [ ] Implement Python-based network diagnostics.
- [ ] Integrate Nmap for network discovery and port scanning.
- [ ] Implement packet capture workflows using TCPDump.
- [ ] Develop packet analysis and traffic inspection functionality.
- [ ] Build automated network monitoring and diagnostic services.
- [ ] Develop REST APIs using FastAPI.
- [ ] Create an interactive monitoring dashboard using React.
- [ ] Configure AWS infrastructure using EC2 and VPC.
- [ ] Integrate CloudWatch for infrastructure monitoring.
- [ ] Implement diagnostic reporting and logging.

## Learning Outcomes

NetScope is also an exploration of practical networking and infrastructure engineering concepts, including:

- TCP/IP networking and network diagnostics.
- Packet capture and protocol analysis.
- Network discovery and service identification.
- Linux administration and Shell scripting.
- Python-based network automation.
- REST API development and system integration.
- Cloud networking and infrastructure monitoring.
- Network security and troubleshooting.

## Security & Responsible Usage

NetScope is intended for educational, diagnostic, and authorised network monitoring purposes.

Network discovery, scanning, and packet capture operations should only be performed on systems and networks owned by the user or where explicit permission has been granted.

## Project Status

NetScope is currently under active development. Features, integrations, and infrastructure components are being implemented incrementally.

---

**Developed by Shruti Yadav**

[GitHub](https://github.com/saoirseros) | [LinkedIn](http://www.linkedin.com/in/shruti-yadav-003b932bb)