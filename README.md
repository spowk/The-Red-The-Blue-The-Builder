# The-Red-The-Blue-The-Builder

### ⚠️ Privacy & Security Disclaimer
For security and anonymity purposes, sensitive data including domain names, passwords, specific usernames, and unapproved IP addresses have been redacted from all reports and screenshots.

### Project Description
A comprehensive home lab project covering Red Team operations, Blue Team monitoring, and infrastructure building using Wazuh SIEM.

### 🏗️ The Builder (Infrastructure & Hardware)
* **Wazuh SIEM Manager:** Hosted on an Intel NUC running Ubuntu (10.0.0.103).
* **Attacker Machine (Red Team):** Hosted on a secondary Intel NUC running Parrot OS (10.0.0.109).
* **Victim Endpoint & SOC Monitor:** A Dell Optiplex 3070 running Windows 11 (10.0.0.104).

![Agent Installation](powershell_instalagent.png)

### 🔴 The Red (Offensive Operations)
* **Reconnaissance:** Network enumeration using Nmap.
![Nmap Scan](before_attack.png)
* **Initial Access:** RDP brute-force and remote access via xfreerdp.
![RDP Attack 1](RDPHASE.png)
![RDP Attack 2](RDPHASEb.png)
![RDP Session](RDPHSASE_on.png)
* **Persistence & Privilege Escalation:** Adding a rogue local administrator account.
![Adding User](cmd_create_hacker.png)

### 🔵 The Blue (Defensive Operations)
* **Wazuh Monitoring:** Real-time detection of brute-force and account modifications.
![SOC Dashboard](project_phase_1soc.png)
* **Threat Intelligence:** Mapping activity to MITRE ATT&CK.
![Attack Tactics](phase1_dashboard.png)
* **Vulnerability & Compliance:** Performing System Configuration Assessment (SCA).
![SCA Scans](final_dashboard.png)
![Victim Status](victim.png)

### 📊 Security Incident Report
This repository includes a raw exported log file (`report.csv`) extracted from the Wazuh SIEM. 
👉 **[Click here to view the full report.csv](report.csv)**
