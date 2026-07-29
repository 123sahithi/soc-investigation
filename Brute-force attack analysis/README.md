# Windows Brute Force Attack Detection

## Overview

This project demonstrates the investigation of a Windows brute-force attack using Windows Security Event Logs.

A large number of failed logon attempts (Event ID 4625) originating from a single IP address were detected within a short period. The attacker successfully authenticated after multiple failed attempts, indicating a compromised account.


## Objectives

- Detect brute-force login attempts
- Analyze Windows Security logs
- Identify attacker IP address
- Create detection logic
- Map activity to MITRE ATT&CK
- Recommend mitigation


## Environment

- Windows 11
- Windows Event Viewer


## Skills Demonstrated

- Log Analysis
- Windows Security Events
- IOC Extraction
- Threat Detection
- MITRE ATT&CK Mapping
- Incident Response


## Detection Summary

| Event | Count |
|--------|------:|
| Event ID 4625 | 24 |
| Event ID 4624 | 1 |


## Final Verdict

Severity: **High**

Attack Type: **Windows Brute Force**

Status: **Contained**
