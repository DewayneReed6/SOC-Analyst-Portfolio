# Project 004 — SSH Authentication Log Investigation

## Investigation Overview

**Role:** Junior SOC Analyst (Training)
**System:** server01
**Log Source:** Simulated Linux SSH authentication logs
**Status:** Initial Investigation Completed

## Objective

Investigate failed and successful SSH authentication
events to identify suspicious login patterns.

## Tools Used

- macOS Terminal
- grep
- awk
- sort
- uniq
- cat

## Evidence Summary

- Total failed logins: 6
- Total successful logins: 2
- Suspicious source IP: 203.0.113.45
- Target account: jsmith
- Failed attempts from suspicious IP: 5
- Successful attempts from suspicious IP: 1
- Time between first failure and success: 15 seconds

## Investigation Findings

The authentication logs revealed five failed SSH
login attempts against the jsmith account.

All five attempts originated from 203.0.113.45
and occurred at three-second intervals.

A successful SSH login from the same IP address
was recorded at 09:00:16.

This pattern could indicate password guessing
or credential misuse.

The available evidence does not establish whether
the successful login was authorized.

## Analyst Assessment

Classification: Suspicious Authentication Activity
Severity: Medium (Training Assessment)

Additional investigation is required to determine
whether the account was compromised.

## Recommended Actions

1. Verify the login with the account owner.
2. Review additional SSH session activity.
3. Check source IP against approved access records.
4. Investigate unusual commands or file access.
5. Escalate if unauthorized access is confirmed.
6. Consider MFA, SSH key authentication, and
   appropriate login rate limiting.

## Conclusion

This investigation demonstrated my ability to
analyze SSH authentication logs using Terminal,
identify suspicious login patterns, and document
security findings without making unsupported claims.

## Training Disclaimer

All log entries and IP addresses are fictional
and used for cybersecurity training purposes.
