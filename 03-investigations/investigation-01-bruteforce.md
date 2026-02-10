# Investigation 01 – Suspected Brute Force Activity

## Summary
Multiple failed logon attempts were detected against a local Windows account over a short time period.

## Alert Source
Detection rule: Brute Force Logon Attempts
Event ID: 4625

## Timeline
- 10:02 – First failed logon attempt
- 10:05 – Alert triggered after threshold reached
- 10:06 – Account temporarily locked

## Evidence
- Repeated Event ID 4625 entries
- Source IP consistent across attempts
- Targeted single user account

## Assessment
Likely automated password guessing against a local account.

## Recommended Actions
- Reset affected user password
- Block source IP at firewall
- Review other accounts for similar activity
- Enable account lockout policies

## Lessons Learned
Improve alert thresholds and correlation with other indicators.
