# SOC Lab Report – Week 3

## Incident Summary
Suspicious activity detected on host 10.0.2.15 involving abnormal outbound traffic and repeated login failures.

## Incident ID
SOC-2026-W3-001

## Severity
High – abnormal outbound traffic with repeated login failures

## Timeline
- Detection: 08 January 2026, 20:15 IST
- Escalation: 08 January 2026, 20:30 IST
- Containment: 08 January 2026, 21:00 IST
- Resolution: 08 January 2026, 21:30 IST

## Evidence
- CSV export and SHA256 hashes documented in [Evidence-Preservation/evidence-notes.md](Evidence-Preservation/evidence-notes.md)

## Alert Triage
Checklist and IOC validation steps documented in [Alert-Triage/triage-checklist.md](Alert-Triage/triage-checklist.md)

## Escalation
Escalation email sent to SOC Lead, documented in [Alert-Management/escalation-email.md](Alert-Management/escalation-email.md)

## Stakeholder Communication
Briefing prepared for non-technical stakeholders in [Capstone-Project/stakeholder-briefing.md](Capstone-Project/stakeholder-briefing.md)

## Impact Assessment
Potential compromise of host 10.0.2.15 with risk of unauthorized access and data exfiltration.

## Lessons Learned
- Importance of maintaining authentic evidence (CSV exports, hashes, triage notes)
- Clear escalation with Incident ID and severity improves tracking
- Linking all artifacts into one report ensures reproducibility
- Documenting timelines strengthens accountability
- Stakeholder briefings improve communication and trust

## Next Steps
- SOC Lead to review and advise on containment
- Reset affected credentials
- Monitor host for persistence attempts
- Continue evidence collection for any new alerts
