# Brute Force Incident Response Playbook

## Purpose
Provide a structured response process for suspected brute force login attempts.

## Detection
Triggered by repeated failed logon events (Event ID 4625).

## Immediate Actions
- Validate alert accuracy
- Identify affected account(s)
- Check for successful logons following failures
- Block suspicious IP addresses

## Containment
- Disable or lock compromised accounts
- Force password resets
- Increase logging temporarily
- Monitor for continued activity

## Eradication & Recovery
- Patch exposed services
- Review firewall rules
- Restore normal account access
- Notify relevant stakeholders

## Post-Incident
- Document findings
- Update detection rules
- Conduct lessons-learned review
