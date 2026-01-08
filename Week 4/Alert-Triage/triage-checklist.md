# Alert Triage – Week 4

## IOC Validation
- Source IP: 203.0.113.45 checked against threat intelligence feeds
- Destination IP: confirmed as suspicious external host
- Host: 10.0.2.25 verified in Wazuh dashboard

## Authentication Failures
- 45 failed SSH login attempts within 10 minutes
- Accounts targeted: root, admin
- No successful login observed during attack window

## Outbound Traffic Review
- Abnormal outbound connection attempts on port 22
- Destination flagged as untrusted
- Traffic volume exceeded baseline thresholds

## Alert Correlation
- Multiple alerts linked to same host and timeframe
- Correlated with detection timeline (08 January 2026, 19:45 IST)

## Analyst Actions
- Preserved logs and CSV export
- Verified hash integrity of evidence
- Escalated incident to SOC Lead at 20:00 IST
