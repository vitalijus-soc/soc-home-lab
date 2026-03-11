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
