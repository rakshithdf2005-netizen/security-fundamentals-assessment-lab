# Security Fundamentals & Vulnerability Assessment Lab

## Project Overview
This repository contains the technical documentation, vulnerability assessment artifacts, and defensive hardening configurations for the Cybersecurity Fundamentals Assessment.

## Author
- **Name:** Rakshith S H
- **Scope:** Modules 1, 2, and 3 Comprehensive Deliverables

## Lab Architecture
- **Environment:** Isolated virtual host-only network (`192.168.56.0/24`)
- **Assessment Workstation:** Kali Linux
- **Target Testbed:** Intentionally vulnerable web applications & network daemons

## Scope & Methodology
Assessments were structured under the **Penetration Testing Execution Standard (PTES)** and **NIST SP 800-115**:
1. **Passive Reconnaissance:** Certificate transparency logs and DNS enumeration.
2. **Active Discovery:** Port scanning via TCP SYN stealth scans (`nmap -sS -sV`).
3. **Vulnerability Analysis:** Identification of legacy daemons and input validation flaws.
4. **Defensive Hardening:** Implementation of prepared statements, least-privilege service accounts, and host-level firewall filtering.

## Findings Summary
| ID | Finding | Target | CVSS v3.1 | Status |
|----|---------|--------|-----------|--------|
| SEC-01 | Unrestricted Anonymous FTP | Port 21/TCP | 7.5 (High) | Mitigated |
| SEC-02 | Default Administrative Credentials | Port 80/TCP | 8.8 (High) | Mitigated |
| SEC-03 | SQL Injection on Search Parameter | Port 80/TCP | 8.6 (High) | Mitigated |

## Documentation
The complete assessment report is available in the `documentation/` directory.
