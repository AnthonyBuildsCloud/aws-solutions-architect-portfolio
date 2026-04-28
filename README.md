# AWS Solutions Architect Portfolio & Study Notes

I’m building practical AWS architecture skills through hands-on labs, structured notes, documented projects, and certification prep as I work toward the **AWS Certified Solutions Architect – Associate (SAA-C03)**.

This repository documents my progression from **AWS Certified Cloud Practitioner (CLF-C02)** into more advanced AWS architecture concepts, service tradeoff analysis, and portfolio-ready cloud projects. My focus is on developing real-world AWS design skills in areas such as **compute, storage, networking, security, resilience, and scalable system design**.

My goal is not only to earn the certification, but to build the kind of cloud architecture foundation that translates into real-world AWS and cloud-focused roles.

---

## Certifications

- **AWS Certified Cloud Practitioner (CLF-C02)** — March 2026  
  [View Certificate](./certifications/aws-certified-cloud-practitioner-clf-c02.pdf)

---

## Completed Training

- **AWS Cloud Practitioner Essentials** — AWS Skill Builder
- **AWS Certified Cloud Practitioner Exam Prep Plan** — AWS Skill Builder
- **AWS Certified Cloud Practitioner (CLF-C02)** — Earned March 2026
- **Stephane Maarek SAA-C03 Sections 1–5** — Completed

---

## Current Focus

- **AWS Certified Solutions Architect – Associate (SAA-C03)**
- **SAA-C03 study roadmap in progress** using Stephane Maarek, Tutorials Dojo, and AWS Skill Builder
- **Currently moving into Section 6: EC2 – Solutions Architect Associate Level**
- Core AWS architecture patterns and service tradeoffs
- Hands-on AWS labs and portfolio projects
- Building stronger documentation, diagrams, and architecture reasoning
- Expanding this repository into a recruiter-facing cloud portfolio

---

## Current Study Progress

### SAA-C03 Course Progress
- **Sections 1–5 completed**
- **Section 4: IAM & AWS CLI quiz score — 8/9**
- **Section 5: EC2 Fundamentals quiz score — 11/12**
- Main weak areas identified:
  - **IAM Security Tools**
  - **EC2 licensing / purchasing scenario judgment**
- Next section: **Section 6 — EC2: Solutions Architect Associate Level**

### Current Weak Areas
- IAM Security Tools
  - IAM Credential Report
  - IAM Access Advisor
  - how MFA fits into IAM account security
  - distinguishing security auditing tools from general IAM best practices
- EC2 licensing and purchasing scenario selection
  - understanding when license-related constraints affect EC2 decisions
  - recognizing scenario clues tied to vendor licensing and instance choice

---

## Architecture Skills Being Built

This repository is focused on developing and documenting skills in:

- **Identity and access management** with IAM
- **Compute design** with EC2, Auto Scaling, and Elastic Load Balancing
- **Storage decisions** across S3, EBS, and EFS
- **Networking fundamentals** with VPCs, subnets, route tables, internet gateways, NAT gateways, and security groups
- **Content delivery and edge architecture** with CloudFront
- **Database selection** across RDS, Aurora, and DynamoDB
- **Security best practices** and least-privilege design
- **High availability, resilience, and cost-aware architecture**

---

## Featured Projects

### Project 01 — Static Website on Amazon S3 + CloudFront
Built and deployed a static website using Amazon S3 for storage and CloudFront for secure delivery over HTTPS.

**Architecture:** Local HTML → Amazon S3 → S3 Static Website Hosting → CloudFront

**What it demonstrates**
- Static website hosting with Amazon S3
- Public access configuration with bucket policies
- CloudFront distribution setup
- HTTPS delivery through CloudFront
- End-to-end AWS deployment workflow

**Why this project matters**  
This project demonstrates foundational AWS architecture skills around storage, content delivery, and secure public web hosting. It also serves as a starting point for future enhancements such as stronger origin protection, custom domain integration, and more production-minded hardening.

[View Project 01](./labs/project-01-static-website/README.md)

---

## Notes Index

- [Module 1 – Introduction to the Cloud](notes/module-01-intro-to-cloud.md)
- [Module 2 – Compute in the Cloud](notes/module-02-compute-in-the-cloud.md)
- [Module 3 – Exploring Compute Services](notes/module-03-exploring-compute-services.md)
- [Module 4 – Going Global](notes/module-04-going-global.md)
- [Module 5 – Networking](notes/module-05-networking.md)
- [Module 6 – Storage](notes/module-06-storage.md)
- [Module 7 – Databases](notes/module-07-databases.md)
- [Module 8 – AI/ML & Data Analytics](notes/module-08-ai-ml-data-analytics.md)
- [Module 9 – Security](notes/module-09-security.md)
- [Module 10 – Monitoring, Compliance, and Governance](notes/module-10-monitoring-compliance-governance.md)
- [Module 11 – Pricing and Support](notes/module-11-pricing-and-support.md)
- [Module 12 – Migrating to the AWS Cloud](notes/module-12-migrating-to-the-aws-cloud.md)
- [Module 13 – Well-Architected Solutions](notes/module-13-well-architected-solutions.md)

---

## Repository Structure

- `notes/` → AWS service breakdowns, module summaries, study notes, weak-area tracking, error logs, and decision notes
- `labs/` → hands-on projects with architecture and screenshots
- `training/` → course progress and training summaries
- `certifications/` → AWS certification proof

---

## Training & Coursework

### Completed
- AWS Cloud Practitioner Essentials (AWS Skill Builder)
- AWS Certified Cloud Practitioner Exam Prep Plan (AWS Skill Builder)
- AWS Certified Cloud Practitioner (CLF-C02)
- SAA-C03 Sections 1–5

### Current
- AWS Certified Solutions Architect – Associate (SAA-C03) preparation
- Section 6: EC2 – Solutions Architect Associate Level
- hands-on AWS architecture projects
- architecture-focused notes and service comparisons
- portfolio and GitHub improvement work

### Primary Study Resources
- Stephane Maarek
- Tutorials Dojo
- AWS Skill Builder
- Adrian Cantrill for deeper review on weak topics

---

## Section Checkpoints

### Section 4 — IAM & AWS CLI
**Status:** Completed  
**Quiz Score:** 8/9

**Key takeaways**
- IAM users represent people or applications needing AWS access
- IAM groups simplify permission management across users
- IAM policies are JSON documents made of permission statements
- IAM roles provide temporary assumed permissions and are preferred for AWS services
- Root account security should include MFA and minimal daily use
- AWS CLI and CloudShell are useful for command-line AWS management

**Main review item**
- IAM Security Tools
  - IAM Credential Report
  - IAM Access Advisor
  - MFA as a critical account protection measure

---

### Section 5 — EC2 Fundamentals
**Status:** Completed  
**Quiz Score:** 11/12

**Key takeaways**
- EC2 is a core AWS compute service used when you need virtual servers and OS-level control
- EC2 purchasing models should match workload needs and cost constraints
- Security Groups act as virtual firewalls for EC2 instances
- EC2 instance types should be chosen based on workload requirements
- EC2 purchasing decisions can involve Reserved Instances, Spot Instances, and On-Demand usage depending on the scenario

**Main review item**
- EC2 licensing and purchasing scenario judgment
  - vendor licensing constraints
  - matching purchase options to workload patterns
  - recognizing when a scenario is not a fit for the cheapest option

---

### Section 6 — EC2: Solutions Architect Associate Level
**Status:** Completed  
**Quiz Score:** 2/5

**Key takeaways**
- ENIs are tied to a subnet and Availability Zone
- EC2 Hibernate preserves RAM state by writing it to the root EBS volume
- Placement groups matter for specialized EC2 placement and communication patterns
- Cluster Placement Groups fit low-latency, high-throughput workloads
- Specialized EC2 features often appear in scenario-heavy SAA questions

**Main review items**
- EC2 Hibernate
- ENI Availability Zone scope
- Placement Group scenario matching

### Section 7 — EC2 Instance Storage
**Status:** Completed  
**Quiz Score:** 7/9

**Key takeaways**
- EBS is persistent block storage for EC2
- instance store is temporary local storage
- AMIs are Region-scoped
- root and additional EBS volumes can behave differently on termination
- high-IOPS workloads require careful EBS volume selection

**Main review items**
- high-performance EBS volume selection
- root volume vs non-root volume behavior

## How I Use This Repo

I use this repository to:

- document AWS concepts in plain English
- capture hands-on labs and project work
- compare AWS services and architecture tradeoffs
- build a visible portfolio of AWS learning and applied practice
- track progress toward AWS Solutions Architect Associate
- strengthen recruiter-facing proof of cloud skills

---

## Next Steps

- Continue through **Section 6: EC2 – Solutions Architect Associate Level**
- Add stronger architecture diagrams and service comparison notes
- Keep turning quiz weak areas into GitHub-ready notes
- Build more advanced AWS projects
- Improve repository structure over time
- Achieve AWS Certified Solutions Architect – Associate (SAA-C03)

---

## Why This Repo Exists

I’m using this repository to make my AWS learning visible, structured, and practical.

Instead of treating certification prep like a private study process, I’m documenting my labs, notes, projects, quiz takeaways, and architecture learning in public as I build toward AWS Solutions Architect Associate and cloud-focused roles.
