# TryHackMe: Cloud Security Fundamentals Lab

## 🔍 Overview
This lab walks through key concepts in cloud security using TryHackMe’s Cloud Fundamentals and Cloud Security rooms. Focus areas include IAM, logging, misconfigurations, and basic incident response.

---

## ☁️ Cloud Concepts Reviewed
- **IaaS**: EC2, virtual machines, and storage
- **PaaS**: Managed database services (e.g., AWS RDS)
- **SaaS**: Google Workspace, Office 365
- **Public Cloud**: AWS, Azure, GCP
- **Private Cloud**: On-prem solutions managed by org
- **Hybrid Cloud**: Combination of public and private environments

---

## 🔐 IAM & Access Control
- Created IAM users, groups, and roles in AWS
- Applied least privilege principles using IAM policies
- Explored **IAM Role Assumption** and temporary credentials

🛠 Tools Used:
- AWS Console
- AWS CLI

---

## 🪣 S3 Bucket Misconfig Lab
- Identified a misconfigured public S3 bucket
- Used `curl` and `aws s3 ls` to list contents
- Modified bucket policy to restrict public access
- Applied encryption-at-rest and versioning

🛡️ Lessons:
- Misconfigured S3 buckets are a common vector for data leakage
- Bucket policy + ACLs must be reviewed regularly

---

## 🧾 CloudTrail Log Review
- Enabled CloudTrail logging
- Monitored API calls and access logs
- Detected unauthorized access simulation
- Exported logs to S3 for centralized analysis

---

## ⚠️ MITRE ATT&CK Mapping (Cloud Techniques)
| Technique        | Description                                |
|------------------|--------------------------------------------|
| T1078            | Valid Accounts (stolen IAM creds)          |
| T1530            | Data from Cloud Storage                    |
| T1529            | System Shutdown/Reboot in cloud            |

---

## 🔎 Reflections & Next Steps
- Practice log aggregation with ELK or Wazuh
- Explore multi-cloud security posture management (CSPM)
- Implement CloudWatch alerts for privilege escalation events

---

📅 **Completed:** June 2025  
📚 **Platform:** [TryHackMe](https://tryhackme.com/)  
🔗 **Room:** Cloud Security Fundamentals, S3 Bucket Attack
