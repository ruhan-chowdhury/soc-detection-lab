# Detection Rules

This folder contains simple detection logic written for the SOC Detection Lab.

The aim is to identify suspicious behaviour in Windows event logs and document why the activity matters.

## Included Detections

### 1) Brute Force Logon Attempts
- Event ID: 4625
- Condition: More than 10 failed logons within 5 minutes for the same account or IP
- Threat: Password guessing / credential stuffing

### 2) New Local Administrator Account
- Event IDs: 4720 (account created), 4732 (added to local admin group)
- Threat: Privilege escalation and persistence

### 3) Suspicious PowerShell Execution
- Event ID: 4688 (process creation)
- Indicators:
- Encoded commands (-enc)
- IEX / Invoke-Expression
- Downloads from web URLs
- Threat: Malware execution

## Notes
These detections are designed for learning purposes and may require tuning in real environments.
