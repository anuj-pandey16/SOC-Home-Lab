# SOC Home Lab – Wazuh, Splunk & Sysmon Based Threat Detection Environment

## Overview

This project demonstrates the design and implementation of a Security Operations Center (SOC) Home Lab for log collection, threat detection, security monitoring, and incident investigation. The lab simulates a real-world SOC environment using industry-standard tools including Wazuh, Splunk, Sysmon, and Windows Event Logs.

The primary objective of this lab is to gain hands-on experience in Security Monitoring, Detection Engineering, Incident Response, and Threat Hunting by generating and analyzing security events in a controlled environment.

---

## Lab Architecture

Windows 11 Endpoint
↓
Sysmon
↓
Wazuh Agent
↓
Wazuh Manager (Ubuntu Server)
↓
Splunk Universal Forwarder
↓
Splunk SIEM Dashboard

---

## Key Features

* Deployed Wazuh Manager on Ubuntu Server from scratch
* Integrated Windows 11 endpoint with Wazuh Agent
* Configured Sysmon for enhanced endpoint visibility
* Forwarded security logs to Splunk SIEM using Universal Forwarder
* Monitored Windows Security Events and Sysmon Logs
* Created custom dashboards for security monitoring
* Developed detection rules for common attack scenarios
* Investigated alerts and documented incident response procedures

---

## Detection Use Cases

### Brute Force Attack Detection

* Windows Event ID 4625
* Multiple failed authentication attempts
* Account lockout monitoring

### Successful Logon Monitoring

* Windows Event ID 4624
* Detection of suspicious login activity

### PowerShell Execution Detection

* Windows Event ID 4688
* Detection of encoded or suspicious PowerShell commands

### User Account Creation Monitoring

* Windows Event ID 4720
* Detection of unauthorized user creation

### Remote Desktop Activity Monitoring

* Logon Type 10 Events
* Tracking remote access attempts

### Sysmon-Based Process Monitoring

* Process Creation (Event ID 1)
* Network Connections (Event ID 3)
* Image Load Events (Event ID 7)

---

## MITRE ATT&CK Mapping

| Detection Use Case   | ATT&CK Technique |
| -------------------- | ---------------- |
| Brute Force          | T1110            |
| PowerShell Execution | T1059.001        |
| Remote Services      | T1021            |
| Account Discovery    | T1087            |
| Credential Access    | T1003            |

---

## Skills Demonstrated

* Security Operations Center (SOC) Monitoring
* SIEM Administration
* Endpoint Detection & Monitoring
* Log Analysis
* Threat Detection
* Incident Response
* Detection Engineering
* Windows Event Log Analysis
* Sysmon Configuration
* Wazuh Administration
* Splunk Dashboarding
* MITRE ATT&CK Framework

---

## Technologies Used

* Wazuh
* Splunk Enterprise
* Sysmon
* Ubuntu Server
* Windows 11
* VMware Workstation
* Sigma Rules
* MITRE ATT&CK Framework

---

## Future Enhancements

* Sigma Rule Development
* Threat Hunting Scenarios
* Malware Detection Use Cases
* YARA Rule Integration
* Automated Incident Response Playbooks
* Active Directory Monitoring
* Threat Intelligence Integration

---

## Disclaimer

This project was built for educational and research purposes to develop practical SOC analyst skills and understand real-world security monitoring workflows.
