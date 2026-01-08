# Alert Triage – Week 6

## IOC Validation
- Source IP: 203.0.113.60 checked against threat intelligence feeds
- Destination IP: confirmed as suspicious external host
- Host: 10.0.2.40 verified in Wazuh dashboard

## Authentication Failures
- 50 failed SSH login attempts within 10 minutes
- Accounts targeted: root, admin
- No successful login observed

## Outbound Traffic Review
- Abnormal outbound connection attempts on port 22
- Destination flagged as untrusted
- Traffic volume exceeded baseline thresholds

## Alert Correlation
- Multiple alerts linked to same host and timeframe
- Correlated with detection timeline (08 January 2026, 09:30 IST)

## Analyst Actions
- Preserved logs and CSV export
- Verified hash integrity of evidence
- Escalated incident to SOC Lead
