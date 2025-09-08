# Forensics Lab Notes

## Goal
Practice forensic evidence collection & analysis in AWS.

## Steps
1. Snapshot compromised EC2 instance.
2. Mount snapshot to forensic analysis instance.
3. Collect logs from:
   - CloudTrail
   - VPC Flow Logs
   - S3 Access Logs
4. Analyze indicators of compromise (IOCs).

## Observations
- Example: Unusual SSH connections
- Example: Persistence via cron jobs

## Lessons Learned
- Always preserve original evidence
- Automate snapshot & log export process
