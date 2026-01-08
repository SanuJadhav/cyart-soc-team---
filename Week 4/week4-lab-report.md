# SOC Lab Report – Week 4

## Incident Summary
Suspicious activity detected on host 10.0.2.25 involving repeated failed SSH login attempts followed by abnormal outbound traffic to an external IP address.

## Incident ID
SOC-2026-W4-001

## Severity
High – brute force login attempts combined with suspicious outbound connections

## Timeline
- Detection: 08 January 2026, 19:45 IST
- Escalation: 08 January 2026, 20:00 IST
- Containment: 08 January 2026, 20:30 IST
- Resolution: 08 January 2026, 21:15 IST

## Evidence
- CSV export and SHA256 hashes documented in [Evidence-Preservation/evidence-notes.md](Evidence-Preservation/evidence-notes.md)
- Preserved Wazuh alert logs showing repeated SSH failures and outbound traffic

## Alert Triage
Checklist and IOC validation steps documented in [Alert-Triage/triage-checklist.md](Alert-Triage/triage-checklist.md)

## Escalation
Escalation email sent to SOC Lead, documented in [Alert-Management/escalation-email.md](Alert-Management/escalation-email.md)

## Stakeholder Communication
Briefing prepared for non-technical stakeholders in [Capstone-Project/stakeholder-briefing.md](Capstone-Project/stakeholder-briefing.md)

## Impact Assessment
Potential compromise of host 10.0.2.25 with risk of credential theft and unauthorized remote access. Outbound traffic suggests possible data exfiltration attempts.

## Lessons Learned
- Ensure SSH services are hardened with key-based authentication
- Continuous monitoring of failed login attempts is critical
- Outbound traffic anomalies must be escalated quickly
- Documentation of timelines strengthens accountability
- Continue building on Week 3 improvements for reproducibility and authenticity

## Next Steps
- SOC Lead to review and advise on containment
- Reset affected credentials and enforce stronger authentication
- Monitor host for persistence attempts and lateral movement
- Continue evidence collection for any new alerts
- Conduct a post-incident review to improve detection rules
