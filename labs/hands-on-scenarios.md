# Hands-On Scenarios

## Scenario 1: Incident Response Workflow
- Trigger: GuardDuty detects unusual IAM API calls.
- Actions:
  1. Analyze CloudTrail logs.
  2. Identify source IP & user.
  3. Contain by revoking access.
  4. Document incident.

---

## Scenario 2: EC2 Compromise Simulation
- Trigger: EC2 instance mining cryptocurrency.
- Actions:
  1. Quarantine instance using Security Groups.
  2. Take EBS snapshot for forensic analysis.
  3. Terminate infected workload.
  4. Redeploy clean instance.

---

## Scenario 3: S3 Bucket Misconfiguration
- Trigger: Sensitive bucket becomes public.
- Actions:
  1. Detect via AWS Config rule.
  2. Apply block public access.
  3. Run IAM Access Analyzer to verify.
  4. Report incident & lessons learned.
