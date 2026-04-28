# Error Log

This file tracks missed questions, weak reasoning patterns, and review takeaways for SAA-C03 prep.

---

## Entry Template

**Date:**  
**Source:**  
**Topic:**  
**Why I missed it:**  
**Clue I missed:**  
**Correct reasoning:**  
**What I will look for next time:**  

---

## Entry 1

**Date:** 2026-04-18  
**Source:** Stephane Maarek — Section 4 Quiz: IAM & AWS CLI  
**Topic:** IAM Security Tools  
**Why I missed it:** I understood IAM basics well, but I was not fully clear on which named tools AWS uses for IAM security review and auditing.  
**Clue I missed:** The question was asking for a specific IAM security tool, not a broad IAM best practice.  
**Correct reasoning:** IAM security tools include **IAM Credential Report** and **IAM Access Advisor**, which help review credential posture and permission usage. MFA is also a critical IAM-related security control, especially for the root account and privileged users.  
**What I will look for next time:** Distinguish between credential auditing tools, permission usage review tools, and general IAM security best practices.

---

## Entry 2

**Date:** 2026-04-18  
**Source:** Stephane Maarek — Section 5 Quiz: EC2 Fundamentals  
**Topic:** EC2 licensing and purchasing scenario selection  
**Why I missed it:** I understood the EC2 basics overall, but I was less confident when the question introduced vendor licensing constraints and purchasing model tradeoffs in the same scenario.  
**Clue I missed:** The scenario likely included a licensing requirement or limitation that changed which EC2 purchasing option or configuration made the most sense.  
**Correct reasoning:** EC2 purchasing choices should match workload behavior, cost goals, and any licensing restrictions. The cheapest-looking option is not always the right one if the scenario includes license constraints, stability requirements, or long-term workload predictability.  
**What I will look for next time:** Slow down when a question includes licensing details, workload duration, commitment level, or purchasing model language like On-Demand, Reserved, or Spot.

---

## Entry 3

**Date:** 2026-04-18  
**Source:** Stephane Maarek — Section 6 Quiz: EC2 Solutions Architect Associate Level  
**Topic:** EC2 Hibernate  
**Why I missed it:** I was not fully clear on the exact behavior and limits of EC2 hibernation, especially how it differs from stopping or terminating an instance.  
**Clue I missed:** The question was testing detailed behavior, not general EC2 lifecycle knowledge.  
**Correct reasoning:** EC2 hibernation saves the contents of RAM to the root EBS volume so the instance can resume faster later. It is different from stopping because the in-memory state is preserved.  
**What I will look for next time:** Watch for keywords about preserving in-memory application state, faster resume time, and differences between hibernate, stop, and terminate.

---

## Entry 4

**Date:** 2026-04-18  
**Source:** Stephane Maarek — Section 6 Quiz: EC2 Solutions Architect Associate Level  
**Topic:** Elastic Network Interfaces (ENI)  
**Why I missed it:** I understood that ENIs are attachable network interfaces, but I was not fully locked in on their Availability Zone limitation.  
**Clue I missed:** The scenario depended on whether an ENI could be attached across AZ boundaries.  
**Correct reasoning:** An ENI is associated with a subnet, and therefore with a specific Availability Zone. It cannot be attached to an EC2 instance in another AZ.  
**What I will look for next time:** Whenever ENIs appear in a question, check subnet and Availability Zone scope carefully.

---

## Entry 5

**Date:** 2026-04-18  
**Source:** Stephane Maarek — Section 6 Quiz: EC2 Solutions Architect Associate Level  
**Topic:** EC2 Placement Groups  
**Why I missed it:** I was not confident enough in mapping workload type to the correct placement group concept.  
**Clue I missed:** The workload involved big data analysis across a fleet of EC2 instances, which suggests high bandwidth and low latency needs between instances.  
**Correct reasoning:** A Cluster Placement Group is used when EC2 instances need very fast communication and low latency, such as HPC, analytics clusters, or tightly-coupled compute workloads.  
**What I will look for next time:** Watch for workload clues like high-performance computing, tightly-coupled nodes, low latency, and high network throughput between EC2 instances.

---

## Entry 6

**Date:** 2026-04-18  
**Source:** Stephane Maarek — Section 7 Quiz: EC2 Instance Storage  
**Topic:** High-performance EBS volume selection  
**Why I missed it:** I was not fully confident in matching an IOPS-heavy database workload to the correct EBS volume type.  
**Clue I missed:** The scenario specifically mentioned very high IOPS requirements, which should immediately narrow the answer toward a performance-optimized EBS option.  
**Correct reasoning:** When a workload, especially a database, requires very high IOPS, Provisioned IOPS SSD volumes are usually the best fit because they are designed for high-performance, latency-sensitive workloads.  
**What I will look for next time:** Watch for keywords like high IOPS, high-performance database, low latency, and sustained storage performance.

---

## Entry 7

**Date:** 2026-04-18  
**Source:** Stephane Maarek — Section 7 Quiz: EC2 Instance Storage  
**Topic:** Root volume vs additional EBS volume behavior  
**Why I missed it:** I was not fully locked in on how root and non-root EBS volumes behave differently, especially around instance termination.  
**Clue I missed:** The scenario depended on whether the volume was the root volume or an additional attached volume.  
**Correct reasoning:** The root EBS volume is often configured to be deleted on termination by default, while additional EBS volumes are typically not deleted unless explicitly configured that way.  
**What I will look for next time:** Check whether the question is talking about the root volume or a secondary volume, and pay attention to delete-on-termination behavior.

## Current Error Patterns I Want to Watch

- mixing up named AWS security tools with general best practices
- missing scenario clues tied to licensing or purchasing constraints
- rushing when a question sounds familiar instead of isolating the key requirement
- choosing the “cheapest” answer too quickly without checking whether the scenario rules it out

---

## Patterns That Keep Repeating
- TBD
