# NovaShyld Task 3 – Exploitation, Privilege Escalation & Attack Chain Simulation

## Overview

This repository contains the submission for **Task 3** of the NovaShyld Cyber Security Internship.

The objective was to simulate a complete penetration testing attack lifecycle by exploiting a vulnerable service, performing post-exploitation activities, analyzing the generated network traffic, and documenting the entire attack chain.

> **Disclaimer:** This project was performed in a controlled virtual lab environment using Metasploitable2 for educational purposes only.

---

## Objectives

- Perform targeted exploitation using Metasploit Framework
- Gain remote shell access
- Conduct post-exploitation enumeration
- Analyze attack traffic using Wireshark
- Document the complete attack chain

---

## Lab Environment

| Component | Details |
|-----------|---------|
| Attacker Machine | Kali Linux 2025.2 |
| Target Machine | Metasploitable2 |
| Framework | Metasploit |
| Packet Analyzer | Wireshark |
| Network | VirtualBox Host-Only |

---

## Vulnerability Exploited

- **Service:** FTP
- **Software:** vsFTPd 2.3.4
- **Exploit Module:** `exploit/unix/ftp/vsftpd_234_backdoor`

The vulnerable FTP service was identified using Nmap and successfully exploited using Metasploit.

---

## Attack Workflow

1. Reconnaissance
2. Service Enumeration
3. Vulnerability Identification
4. Exploitation using Metasploit
5. Meterpreter Session Establishment
6. Post-Exploitation Enumeration
7. Traffic Capture using Wireshark
8. Attack Chain Documentation

---

## Repository Structure

```
NovaShyld_Task_3/
│
├── Report/
│   └── NovaShyld_Task3_Report.pdf
│
├── Screenshots/
│   ├── 01_msfconsole_launch.png
│   ├── 02_metasploit_module_search.png
│   ├── 03_select_exploit_module.png
│   ├── 04_module_options.png
│   ├── 05_metasploit_configuration.png
│   ├── 06_nmap_service_detection.png
│   ├── 07_exploit_configuration.png
│   ├── 08_exploit_execution.png
│   ├── 09_vsftpd_backdoor_detected.png
│   ├── 10_root_access_verification.png
│   ├── 11_home_directory_listing.png
│   ├── 12_home_directory_enumeration.png
│   ├── 13_network_services.png
│   ├── 14_listening_ports.png
│   ├── 15_sudo_privileges.png
│   ├── 16_privilege_escalation_search.png
│   ├── 17_passwd_file_access.png
│   ├── 18_shadow_file_access.png
│   ├── 19_wireshark_packet_capture.png
│   ├── 20_ip_traffic_filter.png
│   ├── 21_tcp_handshake_analysis.png
│   ├── 22_tcp_port21_filter.png
│   └── 23_ftp_traffic_analysis.png
│
│
├── README.md

```

---

## Tools Used

- Kali Linux
- Metasploit Framework
- Nmap
- Wireshark
- Metasploitable2
- VirtualBox

---

## Key Findings

- Identified vulnerable **vsFTPd 2.3.4** FTP service.
- Successfully exploited the backdoor using Metasploit.
- Obtained a Meterpreter session on the target machine.
- Performed basic system enumeration.
- Captured and analyzed FTP traffic using Wireshark.
- Observed plaintext FTP authentication and exploit-related network activity.

---

## Learning Outcomes

- Vulnerability verification using Nmap
- Exploitation using Metasploit
- Understanding Meterpreter sessions
- Post-exploitation enumeration
- Network traffic analysis
- Attack chain documentation

---

## Author

**Poorvi Goud**

NovaShyld Cyber Security Internship

---

## Disclaimer

This repository is intended solely for educational and ethical cybersecurity training. All activities were conducted in an isolated virtual laboratory using intentionally vulnerable machines. Do not attempt these techniques on systems without explicit authorization.
