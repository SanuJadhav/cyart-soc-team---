# Incident Post-Mortem – Week 2

## Summary
Brief description of the incident.

## Timeline
## Timeline
- Detection: 2026-01-08 20:45 IST
- Escalation: 2026-01-08 20:50 IST
- Containment: 2026-01-08 21:00 IST
- Resolution: 2026-01-08 21:10 IST
## Actions Taken
## Actions Taken
- Conducted triage of Wazuh alerts to confirm suspicious activity
- Preserved evidence (memory dump, Velociraptor CSV, screenshots)
- Escalated incident to SOC lead via email
- Contained activity using CrowdSec firewall rules
- Verified containment by monitoring logs and dashboard
## Lessons Learned
## Lessons Learned
### What Worked
- Quick detection of abnormal outbound traffic via Wazuh alerts
- Effective escalation process with clear communication to SOC lead
- Evidence preservation with hashes and screenshots ensured authenticity
- Containment using CrowdSec firewall rules was successful and timely

### Needs Improvement
- Initial triage took longer due to unclear alert descriptions
- Documentation templates should be pre‑filled to save time during incidents
- More automation needed for hash generation and evidence collection
- Stakeholder briefing could include clearer impact assessment
