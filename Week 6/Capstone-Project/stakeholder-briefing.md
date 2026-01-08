# Stakeholder Briefing – Week 6

## Executive Summary
On 08 January 2026 at 09:30 IST, suspicious activity was detected on host 10.0.2.40. The incident involved repeated failed SSH login attempts followed by abnormal outbound traffic to an external IP address. The SOC team responded promptly to contain the threat.

## Key Findings
- 50 failed SSH login attempts targeting root and admin accounts
- Outbound traffic observed to external IP 203.0.113.60 on port 22
- Evidence preserved (CSV export, SHA256 hash, Wazuh dashboard logs)
- Escalation email sent to SOC Lead

## Business Impact
Potential risk of credential theft and unauthorized access. Outbound traffic suggests possible data exfiltration attempts.

## Actions Taken
- Evidence collected and verified with hash integrity
- Incident escalated to SOC Lead
- Containment measures initiated, including credential reset and monitoring

## Next Steps
- SOC Lead to advise on further containment
- Continue monitoring host 10.0.2.40
- Review SSH authentication policies
- Conduct post-incident review
