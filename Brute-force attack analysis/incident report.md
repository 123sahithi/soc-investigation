# Incident Report

## Incident Summary

| Item | Value |
|------|-------|
| Date | 15 July 2026 |   
| Incident Type | Brute-Force |
| Severity | High |


## Executive Summary

A Windows workstation generated multiple failed authentication attempts within a two-minute period.

Twenty-four failed logons were recorded from a single source IP before one successful login occurred.

The activity matched the behavior of a password brute-force attack.


## Target Host

Hostname

```
WIN11-LAB
```

Operating System

```
Windows 11 Pro
```

User Account

```
Administrator
```

Source IP

```
192.168.1.105
```


## Investigation

### Phase 1

Windows Security Logs showed repeated Event ID 4625 failures.

The same IP repeatedly attempted authentication.


### Phase 2

A successful Event ID 4624 login immediately followed the failures.

This indicates the attacker eventually guessed the password.


## Impact Assessment

- Unauthorized access to the Windows host.
- Compromise of privileged (Administrator) credentials.
- Data theft or unauthorized modification of files.
- Installation of malware or ransomware.
- Lateral movement to other systems within the network.
- Service disruption and potential downtime.
- Increased risk of privilege escalation and persistence.


## Response Actions

- The account was disabled.
- Firewall rules blocked the attacking IP.
- Password reset was completed.
- MFA was enabled.
