# Evidence Notes – Week 5

## CSV Exports
- File: ssh_failures_10.0.2.30.csv
- SHA256: <insert hash>

## Preserved Logs
- Source: Wazuh dashboard
- Event Type: SSH authentication failures
- Count: 60 failed login attempts within 15 minutes
- Outbound Traffic: Connection attempts to external IP 198.51.100.25 on port 22

## Hash Verification
- Integrity of CSV export verified with SHA256

## Additional Evidence
- Alert ID: 2026-SSH-FAIL-W5
- Host: 10.0.2.30
- Severity: High
- Screenshot: Full-window capture preserved in dashboard

## Notes
- Evidence preserved immediately after detection
- Logs retained for reproducibility and authenticity
