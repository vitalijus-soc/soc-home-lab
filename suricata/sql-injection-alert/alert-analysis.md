# SQL Injection Alert Analysis

## Alert Information
Suricata generated an alert indicating a possible SQL injection attempt.

## Investigation Steps
1. Reviewed Suricata eve.json logs
2. Checked source IP address
3. Correlated traffic with nginx access logs
4. Verified HTTP request patterns

## Conclusion
The alert was triggered during a controlled lab simulation.

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
