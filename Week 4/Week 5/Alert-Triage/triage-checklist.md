# Alert Triage – Week 5

## IOC Validation
- Source IP: 198.51.100.25 checked against threat intelligence feeds
- Destination IP: confirmed as suspicious external host
- Host: 10.0.2.30 verified in Wazuh dashboard

## Authentication Failures
- 60 failed SSH login attempts within 15 minutes
- Accounts targeted: root, admin
- No successful login observed

## Outbound Traffic Review
- Abnormal outbound connection attempts on port 22
- Destination flagged as untrusted
- Traffic volume exceeded baseline thresholds

## Alert Correlation
- Multiple alerts linked to same host and timeframe

## Analyst Actions
- Preserved logs and CSV export
- Verified hash integrity of evidence
- Escalated incident to SOC Lead
