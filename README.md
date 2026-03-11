# SOC Home Lab – Blue Team Practice

## About Me

I am building a structured home SOC lab to develop practical skills in:

- Log analysis
- Intrusion detection
- Threat investigation
- Network monitoring
- Incident response fundamentals

## Architecture Diagram

Attack simulation and monitoring pipeline used in this lab:

```
Attacker VM (Kali Linux)
     │
     ▼
Nginx Docker (Docker Container)
     │
     ▼
Suricata IDS
     │
     ▼
Wazuh SIEM
```

## Simulated Threat Scenarios

The following attacks are simulated in this lab environment to generate realistic security alerts and investigation cases.

| Scenario | Description | Detection Tool |
|---------|-------------|---------------|
| SQL Injection Attack | Simulated web application attack against nginx container | Suricata |
| Port Scanning | Network reconnaissance using scanning tools | Suricata |
| SSH Brute Force | Multiple authentication attempts against SSH service | Suricata / Fail2Ban |

## Future Investigations

- Malware traffic detection
- DNS tunneling detection
- Suspicious PowerShell activity

## SOC Investigation Index

This section lists all security investigations performed in this lab environment.

| Attack Type | Description | Investigation |
|-------------|-------------|---------------|
| SQL Injection | Web application attack detected by Suricata | [View Investigation](suricata/sql-injection-alert) |
| Port Scan | Network reconnaissance detected by IDS | [View Investigation](suricata/port-scan-detection) |
| SSH Brute Force | Multiple login attempts detected | [View Investigation](suricata/brute-force-detection) |

## Lab Environment

**Host System**
- Windows 11

**Virtualization**
- VirtualBox

**Virtual Machines**
- Ubuntu Server
- Kali Linux
- Windows testing VM

---

## Security Stack

- Suricata (IDS)
- Wazuh (SIEM)
- Wireshark
- tcpdump
- Fail2Ban
- Docker (nginx attack simulation)
- Sysmon (Windows logging)

---

## Goal

To prepare for a Junior SOC Analyst role by documenting real lab investigations and detection scenarios.
