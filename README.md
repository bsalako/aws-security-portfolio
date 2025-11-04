# AWS Security Portfolio

This repository documents my hands-on journey in **AWS Security**, starting with the **AWS Security Reference Architecture (SRA)** and expanding into projects that demonstrate real-world security practices.  
The goal is to showcase practical skills, not just theory. Each folder contains explanations, screenshots, and eventually automation code that map to AWS security best practices.

---

## 🔐 What is the AWS Security Reference Architecture (SRA)?

The **AWS SRA** is an official blueprint from AWS that provides a **holistic, best-practice design** for securing multi-account AWS environments.  
It covers five key pillars of cloud security:

1. **Identity & Access Management** – Centralized control with AWS Organizations, IAM, and Service Control Policies (SCPs).  
2. **Detection & Response** – Services like GuardDuty, Security Hub, CloudTrail, and CloudWatch for monitoring and incident response.  
3. **Infrastructure Protection** – Network segmentation, WAF, Shield, and VPC security controls.  
4. **Data Protection** – Encryption with KMS, S3 bucket policies, and secure key management.  
5. **Governance, Risk & Compliance** – Aligning with frameworks like CIS, NIST, and FedRAMP.

The SRA is valuable because it shows how **all these services fit together** into a secure, enterprise-ready architecture.

---

## 📸 First Artifact: AWS Organizations

The foundation of the SRA is **AWS Organizations**, which allows you to manage multiple AWS accounts under a single structure.  
This enables:
- Centralized governance  
- Service Control Policies (SCPs)  
- Consolidated billing  
- Delegated security services  

Below is a screenshot of my **AWS Organizations page**, which represents the starting point of my portfolio:

![AWS Organizations Screenshot](organizations.png)

---

## 🚀 Next Steps

- Document how **Service Control Policies (SCPs)** enforce guardrails across accounts.  
- Explore **centralized logging** with CloudTrail + S3 + Athena.  
- Build **Security Hub dashboards** and integrate with Splunk for visibility.  

Each step will include **screenshots, explanations, and (later) automation code** to demonstrate hands-on AWS security expertise.

---

## 📂 Repository Structure

