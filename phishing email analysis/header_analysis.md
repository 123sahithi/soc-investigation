# Email Header Analysis

## Authentication Results

| Authentication | Result |
|---------------|--------|
| SPF | Fail |
| DKIM | Fail |
| DMARC | Fail |


## Sender

support@microsoft-security-alerts.com

Observation:

The sender domain is not owned by Microsoft.


## Reply-To

verify365@gmail.com

Observation:

The Reply-To address differs from the sender address.


## Return Path

support@microsoft-security-alerts.com


## Received IP

185.230.63.186

The IP was checked using AbuseIPDB and showed a suspicious reputation.


## URL Analysis

URL:

https://verify-office365-login.com

Findings

- Fake Microsoft login page
- Credential harvesting
- Multiple security vendors detected phishing


## Attachment Analysis

File

Invoice.html

Purpose

Redirects victims to a phishing website.


## Risk Rating

High

Reasons

- Failed authentication
- Domain impersonation
- Credential harvesting
- Suspicious attachment
