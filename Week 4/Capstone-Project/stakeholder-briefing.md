# Stakeholder Briefing – Week 4

## Executive Summary
On 08 January 2026, suspicious activity was detected on host 10.0.2.25. The incident involved repeated failed SSH login attempts followed by abnormal outbound traffic to an external IP address. The SOC team responded promptly to contain the threat.

## Key Findings
- 45 failed SSH login attempts within 10 minutes targeting root and admin accounts
- Outbound traffic observed to external IP 203.0.113.45 on port 22
- Evidence preserved (CSV export, SHA256 hash, Wazuh dashboard logs)
- Escalation email sent to SOC Lead at 20:00 IST

## Business Impact
Potential risk of credential theft and unauthorized access. Outbound traffic suggests possible data exfiltration attempts, which could impact confidentiality of sensitive information.

## Actions Taken
- Evidence collected and verified with hash integrity
- Incident escalated to SOC Lead
- Containment measures initiated, including credential reset and monitoring for persistence attempts

## Next Steps
- SOC Lead to advise on further containment
- Continue monitoring host 10.0.2.25 for abnormal activity
- Review SSH authentication policies and enforce key‑based login
- Conduct post‑incident review to strengthen detection rules
