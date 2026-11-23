# Project 007 — Phishing Email Investigation

**Role:** Junior SOC Analyst  
**Date:** November 23, 2026  
**Incident Type:** Credential Phishing / Suspected Account Compromise  
**Severity:** High (Simulated)  
**Status:** Investigation Open  
**Environment:** Simulated SOC Training Lab

## 1. Executive Summary

A suspicious phishing email impersonating IT Support targeted four employees. Two emails were delivered, one was quarantined, and one was blocked.

Web proxy logs showed that the Finance employee's device accessed the suspicious phishing website. Shortly afterward, two failed login attempts and one successful login were recorded from the same unfamiliar IP address.

The evidence suggests possible account compromise, but unauthorized access has not been confirmed.

## 2. Phishing Indicators

- Suspicious sender: support@company-security-alert.com
- Return-Path: alerts@unknown-mailer.example
- Phishing URL: company-login-verify.example.com
- Email authentication: SPF failed, DKIM absent, DMARC failed
- Suspicious login source: 198.51.100.42
- Windows Event IDs: 4625 (failed login), 4624 (successful login)

**Note:** Domains and public IP addresses in this exercise are fictional or reserved for documentation.

## 3. Incident Timeline

| Time | Event |
|------|-------|
| 09:16 | Phishing email delivered to Finance |
| 09:20 | Finance accessed suspicious website |
| 09:21 | Failed login from 198.51.100.42 |
| 09:22 | Second failed login from same IP |
| 09:23 | Successful login from same IP |

## 4. Investigation Findings

Email analysis identified an urgent password-expiration message, a suspicious sender domain, and failed authentication checks.

Email gateway logs confirmed that the phishing campaign targeted multiple employees. Finance and HR received the messages.

Web proxy logs showed an allowed connection from Finance to the suspicious domain, while HR's connection attempt was blocked.

Authentication logs recorded two failed logins followed by a successful login involving Finance's account and the same unfamiliar IP address.

These findings indicate suspected account compromise requiring further investigation.

## 5. Severity Assessment

**High Severity — Suspected Account Compromise**

The incident requires urgent investigation because suspicious authentication activity occurred shortly after the phishing website was accessed.

## 6. Recommended Response

1. Escalate the incident to the incident-response team.
2. Preserve phishing emails and relevant security logs.
3. Verify the suspicious login with the Finance employee.
4. Review MFA records and active account sessions.
5. Follow approved account-containment procedures if unauthorized access is suspected.
6. Investigate other recipients and block the phishing domain as appropriate.
7. Continue monitoring for suspicious activity.

## 7. Conclusion

The simulated investigation identified a phishing campaign affecting multiple employees and suspicious authentication activity involving the Finance account.

Although compromise remains unconfirmed, the evidence supports escalation and further investigation.

## Skills Demonstrated

- Phishing Email Analysis
- Email Header Investigation
- Web Proxy Log Analysis
- Windows Event Log Analysis
- Incident Timeline Reconstruction
- Incident Severity Assessment
- SOC Incident Documentation
# Project 007 — Phishing Email Investigation

**Role:** Junior SOC Analyst  
**Date:** November 23, 2026  
**Incident Type:** Credential Phishing / Suspected Account Compromise  
**Severity:** High (Simulated)  
**Status:** Investigation Open  
**Environment:** Simulated SOC Training Lab

## 1. Executive Summary

A suspicious phishing email impersonating IT Support targeted four employees. Two emails were delivered, one was quarantined, and one was blocked.

Web proxy logs showed that the Finance employee's device accessed the suspicious phishing website. Shortly afterward, two failed login attempts and one successful login were recorded from the same unfamiliar IP address.

The evidence suggests possible account compromise, but unauthorized access has not been confirmed.

## 2. Phishing Indicators

- Suspicious sender: support@company-security-alert.com
- Return-Path: alerts@unknown-mailer.example
- Phishing URL: company-login-verify.example.com
- Email authentication: SPF failed, DKIM absent, DMARC failed
- Suspicious login source: 198.51.100.42
- Windows Event IDs: 4625 (failed login), 4624 (successful login)

**Note:** Domains and public IP addresses in this exercise are fictional or reserved for documentation.

## 3. Incident Timeline

| Time | Event |
|------|-------|
| 09:16 | Phishing email delivered to Finance |
| 09:20 | Finance accessed suspicious website |
| 09:21 | Failed login from 198.51.100.42 |
| 09:22 | Second failed login from same IP |
| 09:23 | Successful login from same IP |

## 4. Investigation Findings

Email analysis identified an urgent password-expiration message, a suspicious sender domain, and failed authentication checks.

Email gateway logs confirmed that the phishing campaign targeted multiple employees. Finance and HR received the messages.

Web proxy logs showed an allowed connection from Finance to the suspicious domain, while HR's connection attempt was blocked.

Authentication logs recorded two failed logins followed by a successful login involving Finance's account and the same unfamiliar IP address.

These findings indicate suspected account compromise requiring further investigation.

## 5. Severity Assessment

**High Severity — Suspected Account Compromise**

The incident requires urgent investigation because suspicious authentication activity occurred shortly after the phishing website was accessed.

## 6. Recommended Response

1. Escalate the incident to the incident-response team.
2. Preserve phishing emails and relevant security logs.
3. Verify the suspicious login with the Finance employee.
4. Review MFA records and active account sessions.
5. Follow approved account-containment procedures if unauthorized access is suspected.
6. Investigate other recipients and block the phishing domain as appropriate.
7. Continue monitoring for suspicious activity.

## 7. Conclusion

The simulated investigation identified a phishing campaign affecting multiple employees and suspicious authentication activity involving the Finance account.

Although compromise remains unconfirmed, the evidence supports escalation and further investigation.

## Skills Demonstrated

- Phishing Email Analysis
- Email Header Investigation
- Web Proxy Log Analysis
- Windows Event Log Analysis
- Incident Timeline Reconstruction
- Incident Severity Assessment
- SOC Incident Documentation# Project 007 — Phishing Email Investigation

**Role:** Junior SOC Analyst  
**Date:** November 23, 2026  
**Incident Type:** Credential Phishing / Suspected Account Compromise  
**Severity:** High (Simulated)  
**Status:** Investigation Open  
**Environment:** Simulated SOC Training Lab

## 1. Executive Summary

A suspicious phishing email impersonating IT Support targeted four employees. Two emails were delivered, one was quarantined, and one was blocked.

Web proxy logs showed that the Finance employee's device accessed the suspicious phishing website. Shortly afterward, two failed login attempts and one successful login were recorded from the same unfamiliar IP address.

The evidence suggests possible account compromise, but unauthorized access has not been confirmed.

## 2. Phishing Indicators

- Suspicious sender: support@company-security-alert.com
- Return-Path: alerts@unknown-mailer.example
- Phishing URL: company-login-verify.example.com
- Email authentication: SPF failed, DKIM absent, DMARC failed
- Suspicious login source: 198.51.100.42
- Windows Event IDs: 4625 (failed login), 4624 (successful login)

**Note:** Domains and public IP addresses in this exercise are fictional or reserved for documentation.

## 3. Incident Timeline

| Time | Event |
|------|-------|
| 09:16 | Phishing email delivered to Finance |
| 09:20 | Finance accessed suspicious website |
| 09:21 | Failed login from 198.51.100.42 |
| 09:22 | Second failed login from same IP |
| 09:23 | Successful login from same IP |

## 4. Investigation Findings

Email analysis identified an urgent password-expiration message, a suspicious sender domain, and failed authentication checks.

Email gateway logs confirmed that the phishing campaign targeted multiple employees. Finance and HR received the messages.

Web proxy logs showed an allowed connection from Finance to the suspicious domain, while HR's connection attempt was blocked.

Authentication logs recorded two failed logins followed by a successful login involving Finance's account and the same unfamiliar IP address.

These findings indicate suspected account compromise requiring further investigation.

## 5. Severity Assessment

**High Severity — Suspected Account Compromise**

The incident requires urgent investigation because suspicious authentication activity occurred shortly after the phishing website was accessed.

## 6. Recommended Response

1. Escalate the incident to the incident-response team.
2. Preserve phishing emails and relevant security logs.
3. Verify the suspicious login with the Finance employee.
4. Review MFA records and active account sessions.
5. Follow approved account-containment procedures if unauthorized access is suspected.
6. Investigate other recipients and block the phishing domain as appropriate.
7. Continue monitoring for suspicious activity.

## 7. Conclusion

The simulated investigation identified a phishing campaign affecting multiple employees and suspicious authentication activity involving the Finance account.

Although compromise remains unconfirmed, the evidence supports escalation and further investigation.

## Skills Demonstrated

- Phishing Email Analysis
- Email Header Investigation
- Web Proxy Log Analysis
- Windows Event Log Analysis
- Incident Timeline Reconstruction
- Incident Severity Assessment
- SOC Incident Documentation
