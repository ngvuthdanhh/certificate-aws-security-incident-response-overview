# AWS IR Playbooks

## Playbook 1: Unauthorized IAM Access
- **Detection:** GuardDuty → Anomalous API calls
- **Containment:** Disable compromised IAM credentials
- **Eradication:** Rotate all associated keys, enforce MFA
- **Recovery:** Re-enable user with new policies
- **Post-Incident:** Update IAM policy baseline

---

## Playbook 2: Compromised EC2 Instance
- **Detection:** CloudWatch → CPU spike / GuardDuty → CryptoMiner finding
- **Containment:** Isolate instance via Security Group
- **Eradication:** Terminate malicious processes
- **Recovery:** Restore from clean AMI, patch vulnerabilities
- **Post-Incident:** Strengthen monitoring & alerts

---

## Playbook 3: S3 Data Exposure
- **Detection:** AWS Config non-compliant rule
- **Containment:** Block public access, update bucket policy
- **Eradication:** Identify & remove sensitive leaked files
- **Recovery:** Rebuild with proper access controls
- **Post-Incident:** Automate compliance rules
