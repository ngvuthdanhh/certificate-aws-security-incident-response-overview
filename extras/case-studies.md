# Case Studies – AWS Security Incident Response

## Case Study 1: Unauthorized IAM Access
- **Incident:** Compromised IAM user credentials leaked on GitHub.
- **Response:**
  - Detected via GuardDuty anomaly.
  - Immediate IAM user deactivation.
  - Root cause: No MFA + long-lived keys.
- **Lesson Learned:** Enforce MFA, rotate keys, monitor GitHub for secret leaks.

---

## Case Study 2: EC2 Malware Infection
- **Incident:** EC2 instance used for crypto-mining.
- **Response:**
  - Detected unusual CPU usage in CloudWatch.
  - Contained by isolating the instance with a new Security Group.
  - Forensic analysis via EBS snapshot.
- **Lesson Learned:** Implement workload baselining, automated anomaly detection.

---

## Case Study 3: S3 Data Exfiltration
- **Incident:** Sensitive S3 bucket set to public.
- **Response:**
  - Discovered through AWS Config compliance rule.
  - Bucket policy corrected, public access blocked.
  - Post-incident review revealed misconfiguration.
- **Lesson Learned:** Enforce least privilege, automate compliance checks.
