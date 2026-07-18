# Incident Report

## Incident Summary

| Field | Value |
|--------|-------|
| Incident Type | Phishing |
| Severity | High |


## Executive Summary

A suspicious email claiming to originate from Microsoft Security Team was reported by a user. The email requested immediate verification of the user's Microsoft 365 account due to unusual sign-in activity.


## Email Details

Subject:

Microsoft 365 Account Verification Required

From:

support@microsoft-security-alerts.com

Reply-To:

verify365@gmail.com

Attachment:

Invoice.html


## Root Cause

The attacker spoofed Microsoft's branding and used social engineering techniques to trick users into entering credentials on a fake login page.


## Phishing Indicators

- Sender domain
- Failed SPF, DKIM, and DMARC authentication
- Fake Microsoft login page
- HTML attachment
- Credential harvesting attempt


## Impact Assessment

Potential Impact

- Credential theft
- Unauthorized Microsoft 365 access
- Business Email Compromise (BEC)
- Data leakage


## Response Actions

- Block sender domain
- Block phishing URL
- Notify users
- Reset passwords (if clicked)
- Enable MFA
