# Weak Areas

This file tracks recurring weak topics from quizzes, section reviews, and practice exams while I prepare for the AWS Certified Solutions Architect – Associate (SAA-C03).

## Current Weak Areas

### Section 4 — IAM & AWS CLI
- IAM Security Tools
  - IAM Credential Report
  - IAM Access Advisor
  - how MFA fits into IAM account security
  - distinguishing security auditing tools from general IAM best practices

### Section 5 — EC2 Fundamentals
- EC2 licensing and purchasing scenario selection
  - understanding when license-related constraints affect EC2 decisions
  - recognizing scenario clues tied to vendor licensing and instance choice
  - matching EC2 purchasing models to workload patterns

### Section 6 — EC2: Solutions Architect Associate Level
- EC2 Hibernate
  - when hibernation is supported
  - how hibernation differs from stop and terminate
  - when hibernation is useful in real scenarios
- Elastic Network Interfaces (ENI)
  - ENIs are tied to a subnet and AZ
  - ENIs cannot be attached across Availability Zones
  - understand when a secondary network interface is useful
- EC2 Placement Groups
  - Cluster Placement Group for low-latency / high-throughput workloads
  - recognize HPC / big data / tightly-coupled workload clues
  - distinguish placement group use cases from general EC2 scaling scenarios
 
  ### Section 7 — EC2 Instance Storage
- High-performance EBS volume selection
  - recognize when a workload needs high IOPS
  - know when Provisioned IOPS SSD volumes are the better fit
  - distinguish performance-focused storage questions from general-purpose storage questions
- EBS volume behavior on EC2 instances
  - root volume vs additional attached EBS volumes
  - what happens to volumes on instance termination
  - default delete-on-termination behavior for root volumes vs non-root volumes

## Update Rules
- Add new weak areas after each section quiz
- Keep items short and specific
- Remove or move items down once they feel strong and consistently understood
