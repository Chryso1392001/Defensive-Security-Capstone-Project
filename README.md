# 🛡️ Defensive Security Capstone Project

## 🔍 Focus: PSAD (Port Scan Attack Detector)

This project demonstrates how to detect and block TCP SYN scan attacks using **PSAD**, combined with `iptables`, email alerting, and automated IP blocking.

### 💡 Key Features

- **Port Scan Detection**: Detected aggressive SYN scans using `psad` with iptables logging.
- **Auto-Blocking**: Configured `psad` to automatically block attacker IPs at danger level 3.
- **Alerting**: Integrated Gmail SMTP via `msmtp` to send real-time alerts to the security analyst.
- **Forensics**: Used `tcpdump`, `Wireshark`, and logs from `/var/log/` for trace analysis.
- **Additional Hardening**: Implemented `Fail2Ban` for SSH brute force protection.
- **SIEM Monitoring**: Integrated with **Wazuh** to simulate a real SOC environment.

### 🧪 Attack Simulation

- Nmap command used from Kali:  
  `nmap -sS -T4 -p 1-1000 192.168.81.161`

### 🛠 Tools Used

- PSAD, IPTables, Nmap, Msmtp, Mailutils  
- Kali Linux, Ubuntu Server  
- Wazuh (SIEM), Fail2Ban, Wireshark  


⚠️ _This lab was conducted in a controlled environment using virtual machines. No real systems were harmed._

