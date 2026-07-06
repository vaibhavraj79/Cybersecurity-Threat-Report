# 🛡️ Cybersecurity Threat Intelligence Report — Task 1

## 📋 Overview
This is a professional Threat Intelligence Report prepared as part of the
**Maincrafts Technology Cybersecurity Analyst Internship Program**.

## 📌 Topics Covered
- Introduction to Cybersecurity
- 5 Major Modern Cyber Threats (2024–2025)
- Impact Analysis (Individuals & Organizations)
- Real-World Case Studies
- Preventive Measures & Defense Strategies
- Conclusion & Future Scope

## 🔍 Threats Analyzed
| # | Threat | Key Tool/Method |
|---|--------|----------------|
| 1 | AI-Powered Phishing Attacks | Deepfakes, LLMs |
| 2 | Ransomware-as-a-Service (RaaS) | LockBit, WannaCry |
| 3 | Cloud Security Misconfigurations | AWS, Azure, GCP |
| 4 | IoT Vulnerabilities | Mirai Botnet |
| 5 | Zero-Day Exploits | SolarWinds, MOVEit |

## 📁 File
- [Click here to view Report](https://github.com/vaibhavraj79/Cybersecurity-Threat-Report/blob/main/Cybersecurity_Threat_Report_Task1_vaibhav.pdf)

## 🏢 Organization
Maincrafts Technology Internship Program — June 2025

## 👤 Author
**Vaibhav Raj Singh Rathore** | Cybersecurity Analyst Intern

## 🧪 Task 2 — Personal Cybersecurity Lab Setup
📄 Overview
This task involved building a personal, isolated cybersecurity lab using VirtualBox, hosting an intentionally vulnerable target system (OWASP Juice Shop) alongside a Kali Linux attacker machine, connected via a Host-Only network. The goal was to create a safe, offline environment for practicing hands-on security testing without touching real-world systems.
📌 Topics Covered

Virtual machine setup (Kali Linux + Ubuntu Server)
Docker container deployment (OWASP Juice Shop)
VirtualBox Host-Only networking configuration
Firewall (UFW) rule management
Network troubleshooting (Docker conflicts, manual IP assignment)

🛠️ Steps Performed

Installed and configured Kali Linux and Ubuntu Server VMs in VirtualBox.
Set up a Host-Only network adapter to isolate lab traffic from the host machine and internet.
Deployed OWASP Juice Shop as a Docker container on the Ubuntu target VM.
Configured UFW firewall rules to allow traffic on the required port (3000).
Resolved technical issues including Docker network conflicts and manual static IP assignment using VBoxManage.
Verified connectivity between Kali and the target VM across the Host-Only network.
Documented the full setup process with screenshots for submission.
📎 Deliverable: https://github.com/vaibhavraj79/Cybersecurity-Threat-Report/blob/main/Task2_Lab_Report_Final.pdf

## 🔎 Task 3 — Vulnerability Scanning & Assessment
📄 Overview
Building on the lab environment from Task 2, this task focused on performing a professional-grade vulnerability assessment against the OWASP Juice Shop target — identifying open ports, misconfigurations, and information-disclosure weaknesses using industry-standard reconnaissance tools, without performing active exploitation.
📌 Topics Covered

Network reconnaissance and host discovery
Port and service enumeration
Web server misconfiguration scanning
Hidden endpoint / directory discovery
Manual verification of automated scanner findings
Formal Vulnerability Assessment Report (VAR) writing

🛠️ Steps Performed

Host Discovery — Used Nmap (-sn) to confirm the target VM was reachable on the lab network.
Port & Service Enumeration — Ran a full TCP port scan (-sV -p-) to identify open ports and running services.
Web Vulnerability Scanning — Used Nikto to detect missing security headers, CORS misconfiguration, and other web-layer issues.
Hidden Endpoint Discovery — Used Dirsearch to brute-force hidden files and directories, then manually verified each positive hit in-browser.
Evidence Collection — Saved all raw scan outputs and screenshots as supporting evidence.
Reporting — Compiled all findings into a formal Vulnerability Assessment Report, including severity ratings, impact analysis, and remediation guidance for each issue.

🔑 Key Findings

Open directory listing on /ftp exposing backup and credential-related files (High)
Publicly exposed internal metrics endpoint (/metrics) (Medium)
Missing HTTP security headers (CSP, HSTS, Referrer-Policy) (Medium)
Permissive CORS policy (Medium)
Build metadata disclosure via /stats.json (Low)
Information leak via custom X-Recruiting header (Low)

deliverable:https://github.com/vaibhavraj79/Cybersecurity-Threat-Report/blob/main/Task3_Vulnerability_Assessment_Report.docx
