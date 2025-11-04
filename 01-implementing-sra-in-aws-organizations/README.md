# Implementing the AWS Security Reference Architecture (SRA) in AWS Organizations

## 🔐 Overview
The AWS Security Reference Architecture (SRA) provides a best-practice blueprint for securing multi-account AWS environments.  
The foundation of the SRA is **AWS Organizations**, which enables centralized governance, account management, and security guardrails.

## 🏗️ Why AWS Organizations?
- Centralized account management for workloads, security, and shared services
- Ability to apply **Service Control Policies (SCPs)** across accounts
- Delegated administration for security services (e.g., Security Hub, GuardDuty)
- Consolidated billing and governance

## 📸 My AWS Organizations Setup
Below is a screenshot of my AWS Organizations page, which represents the starting point of my SRA implementation:

![AWS Organizations Screenshot](organizations.png)

## 🧩 Mapping to the SRA
- **Identity & Access Management** → Root OU, SCPs, IAM guardrails
- **Detection & Response** → Delegated GuardDuty and Security Hub accounts
- **Infrastructure Protection** → Network/security OUs for segmentation
- **Data Protection** → Centralized KMS key policies across accounts
- **Governance** → SCPs enforcing compliance (e.g., deny disabling CloudTrail)

## 🚀 Next Steps
- Implement baseline SCPs (e.g., deny disabling CloudTrail, restrict regions)
- Delegate Security Hub and GuardDuty to the Security OU
- Configure centralized logging with CloudTrail + S3 + Athena
