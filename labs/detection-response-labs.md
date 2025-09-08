# Detection & Response Labs

## Lab 1: GuardDuty Findings
- Enable GuardDuty in AWS account.
- Trigger sample findings (IAM anomaly, EC2 compromise).
- Practice triaging alerts.

## Lab 2: CloudTrail Analysis
- Enable CloudTrail across regions.
- Query suspicious activity using Athena.
- Correlate with IAM events.

## Lab 3: Incident Containment with Lambda
- Write Lambda function to auto-isolate compromised EC2.
- Trigger isolation via GuardDuty event → EventBridge → Lambda.

## Lab 4: Forensics in AWS
- Take snapshot of compromised EC2.
- Mount snapshot to forensic instance.
- Analyze artifacts & logs.

## Lab 5: Post-Incident Reporting
- Document timeline of detection, response, recovery.
- Share report with key stakeholders.
