# Port Scan Detection Investigation

## Alert Overview
Suricata triggered an alert indicating possible network reconnaissance activity.

## Observed Activity
Multiple connection attempts were detected from a single source IP targeting multiple ports on the web server.

Example alert:

[**] ET SCAN Potential Port Scan [**]

Source IP: 192.168.0.25  
Destination IP: 192.168.0.10

## Investigation Steps
1. Checked Suricata alerts in eve.json
2. Verified repeated connection attempts
3. Reviewed nginx access logs
4. Confirmed scanning behaviour using nmap in lab simulation

## Conclusion
Activity was generated during controlled lab testing to simulate reconnaissance behaviour.

## Incident Timeline

| Time | Event |
|-----|------|
| 20:14:22 | Suricata triggered SQL Injection alert |
| 20:14:23 | Suspicious HTTP request detected |
| 20:14:25 | Request logged in nginx access log |
| 20:14:30 | Analyst started investigation |
| 20:16:00 | Attack confirmed as simulated SQL injection |

## Analyst Notes
This investigation was performed in a controlled lab environment for educational purposes.
