# SOC Lab Report – Week 5

## Incident Summary
Suspicious activity detected on host 10.0.2.30 involving repeated failed SSH login attempts followed by abnormal outbound traffic to an external IP address. The SOC team investigated, preserved evidence, and escalated the incident for containment.

## Incident ID
SOC-2026-W5-001

## Severity
High – brute force login attempts combined with suspicious outbound connections

## Timeline
- Detection: 08 January 2026, 09:30 IST
- Escalation: 08 January 2026, 10:00 IST
- Containment: 08 January 2026, 10:30 IST
- Resolution: 08 January 2026, 11:15 IST

## Evidence
- CSV export and SHA256 hashes documented in [Evidence-Preservation/evidence-notes.md](Evidence-Preservation/evidence-notes.md)
- Preserved Wazuh alert logs showing repeated SSH failures and outbound traffic

## Alert Triage
Checklist and IOC validation steps documented in [Alert-Triage/triage-checklist.md](Alert-Triage/triage-checklist.md)

## Escalation
Escalation email documented in [Alert-Management/escalation-email.md](Alert-Management/escalation-email.md)

## Stakeholder Communication
Briefing prepared in [Capstone-Project/stakeholder-briefing.md](Capstone-Project/stakeholder-briefing.md)

## Impact Assessment
Potential compromise of host 10.0.2.30 with risk of credential theft and unauthorized access. Outbound traffic suggests possible data exfiltration attempts.

## Lessons Learned
- Harden SSH with key-based authentication
- Monitor failed login attempts continuously
- Escalate outbound traffic anomalies quickly
- Document workflows for reproducibility

## Next Steps
- SOC Lead to review containment
- Reset affected credentials
- Monitor host for persistence attempts
- Conduct post-incident review to improve detection rules
