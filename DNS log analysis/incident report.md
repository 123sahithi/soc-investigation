# Incident Report

## Incident Summary

| Item | Value |
|------|-------|
| Severity | High |
| Incident Type | DNS Beaconing |


## Executive Summary

DNS monitoring, repeated DNS queries were observed from a Windows endpoint to a suspicious external domain.

The queries occurred at regular 60-second intervals, suggesting automated communication rather than normal user activity.

Threat intelligence confirmed the domain had been recently registered and associated with malicious activity.


## Affected Host

Hostname

WIN11-LAB

IP Address

192.168.1.101


## Suspicious Domain

update-microsoft-login.com


## Investigation

- DNS query frequency analyzed
- WHOIS lookup performed
- VirusTotal reputation checked
- Endpoint reviewed for malicious processes
- Network communication monitored


## Potential Impact

- Unauthorized communication with an external command-and-control (C2) server.
- Potential data exfiltration through DNS or follow-on network connections.
- Malware persistence on the affected endpoint.
- Increased risk of lateral movement to other systems.
- Exposure of sensitive organizational information.
- Degradation of network security and trust.


## Response Actions

- Isolated the endpoint from the network to prevent further communication.
- Blocked the malicious domain and associated IP address at the firewall and DNS filtering solution.
- Initiated a full antivirus and endpoint detection (EDR) scan.
- Reviewed running processes, scheduled tasks, and startup entries for persistence mechanisms.
