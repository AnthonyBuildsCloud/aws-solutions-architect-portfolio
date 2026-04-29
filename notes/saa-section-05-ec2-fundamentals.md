# Section 5 — EC2 Fundamentals

## Status
Completed

## Quiz Score
11/12

## Section Summary
This section introduced Amazon EC2 fundamentals, including instance setup, AMIs, instance types, purchasing options, Security Groups, SSH, EC2 Instance Connect, EC2 roles, and broader EC2 basics relevant to architecture decisions.

---

## Key Concepts Covered

- EC2 Basics
- EC2 Instance Types
- Security Groups
- SSH
- EC2 Instance Connect
- EC2 Roles
- EC2 Purchasing Options
- Spot Instances and Spot Fleets
- Public IP vs Private IP basics
- EC2 use case fundamentals

---

## Key Takeaways

### EC2 Basics
- EC2 is a core AWS compute service
- It is used when you need virtual servers and OS-level control
- EC2 is flexible, but requires more management than serverless or fully managed services

### AMIs
- An AMI is a machine image used to launch EC2 instances
- AMIs define the OS, software, and launch configuration baseline
- AMI choice affects how quickly an instance can be provisioned

### Instance Types
- EC2 instance types are chosen based on workload needs
- Different instance families are optimized for different use cases like general purpose, compute optimized, memory optimized, or storage optimized

### Security Groups
- Security Groups act as virtual firewalls for EC2 instances
- They control inbound and outbound traffic
- They are stateful

### EC2 Roles
- EC2 instances can use IAM roles to access AWS services securely
- Roles are preferred over embedding access keys inside applications

### EC2 Purchasing Options
- On-Demand is flexible and good for short-term or unpredictable workloads
- Reserved options are better for steady, predictable workloads
- Spot Instances are best when interruptions are acceptable
- Purchasing model choice should be based on workload behavior, risk tolerance, and cost goals

### Spot Instances and Spot Fleets
- Spot can be highly cost-effective
- Spot is not ideal for workloads that cannot tolerate interruption
- Spot Fleets can combine capacity strategies across instance types and Availability Zones

---

## Main Review Item

### EC2 licensing and purchasing scenario judgment
- vendor licensing constraints
- matching purchase options to workload patterns
- recognizing when a scenario is not a fit for the cheapest option

---

## High-Yield Takeaways
- EC2 is used when OS-level control is needed
- Security Groups protect EC2 instances at the instance level
- IAM roles are preferred over hardcoded credentials
- Instance type selection should match workload requirements
- Purchasing options should match workload predictability and interruption tolerance

---

## Common Exam Traps
- choosing Spot for workloads that cannot be interrupted
- focusing only on cost and ignoring workload behavior
- choosing EC2 when a managed or serverless service is a better fit
- overlooking licensing constraints in architecture scenarios

---

## Quiz Result Reflection
I scored **11/12** on this section quiz. My main weak area was **EC2 licensing and purchasing scenario selection**, especially when licensing constraints affect which purchasing option is appropriate.

---

## What I Need to Review Again
- Spot vs Reserved vs On-Demand scenario selection
- licensing-related EC2 scenario clues
- when cheapest is not actually the correct answer
