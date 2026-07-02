# WAZUH SOC Home Lab

A personal Security Operation Center (SOC) project built to gain hands-on experience with endpoint monitoring, threat detection, log analysis, and incident response using Wazuh

## Overview

- This project documents my journey of building a fully functional SOC environment from scratch using Wazuh v4.13.1
- The objective is to simulate how security analysts monitor endpoints, investigate alerts, and respond to security incidents in a real entreprise environment.
- The lab consists of an Ubuntu server acting as the Wazuh Manager and a Windows 11 endpoint running the Wazuh Agent.

---

# Lab Environment 

|Component  | Technology |
|-----------|---------|
|Hypervisor | Oracle VirtualBox |
|Server OS | Ubuntu Server 24.04 LTS |
|Endpoint OS | Windows 11 Pro |
|SIEM Platform | Wazuh 4.13.1 |
|Dashboard | Wazuh Dashboard |
|Indexer | Wazuh Indexer |
|Agent | Wazuh Windows Agent |

---

# Architecture

            Windows 11 Endoint
            +------------------+
            |    Wazuh Agent   |
            +------------------+
                      |
              TLS (1514/ 1515)
                      |
      +-----------------------------------+
      | Ubuntu Server 24.04 LTS           |
      |-----------------------------------|
      | Wazuh Manager                     |
      | Wazuh Indexer                     |
      | Wazuh Dashboard                   |
      +-----------------------------------+
                      |
                HTTPS (5601)
                      |
             Web Browser Dashboard

---

# Completed Phases

- Ubuntu Server Installation
- Static IP configuration
- Wazuh Installation
- Wazuh Manager configuration
- Wazuh Dashboard configuration
- Wazuh Indexer deployment
- Windows Agent Installation
- Agent Registration
- Secure TLS communication
- File Integrity Monitoring (FIM)
- Security Configuration Assessment (SCA)
- Dashboard verification

# Skills Demonstrated

- Linux Administration
- Virtualization
- Network Configuration
- SSH
- System Installation
- Windows Administration
- SIEM Deployment
- Enpoint Monitoring
- Log Analysis
- Threat Detection
- Security Monitoring
- Incident Response Fundamentals

---

# Repository Structure

SOC-Home-Lab/
|---README.md
|---docs/
|---screenshots/
|---diagrams/
|---reports/
|---detections/
|___scripts/

---

# Future Improvements

- Deploy Sysmon
- Integrate Sysmon with Wazuh
- Deploy Kali Linux attacker VM
- Simulate Brute Force attacks
- Detect Powershell attacks
- Detect malware execution
- Build Custom Detection Rules
- Sigma Rules Integration
- MITRE ATT&CK Mapping
- Incident Ivestigation Playbooks

---

# Author

**HAMADOU AHMADOU**
Bachelor of Security Technology Student
Multimedia University (MMU)
Malaysia















