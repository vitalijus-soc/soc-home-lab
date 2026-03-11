# Brute Force Attack Detection

## Alert Overview
Suricata generated alerts indicating repeated authentication attempts.

## Observed Activity
Multiple login attempts were detected from the same source IP within a short time period.

Source IP: 192.168.0.25  
Destination: SSH service

## Investigation Steps
1. Reviewed Suricata alert logs
2. Checked authentication logs
3. Correlated timestamps
4. Verified repeated login attempts

## Conclusion
Activity was generated during lab simulation of brute force attack using Hydra.

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
