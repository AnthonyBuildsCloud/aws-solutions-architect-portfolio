# Section 6 — EC2: Solutions Architect Associate Level

## Status
Completed

## Quiz Score
2/5

## Section Summary
This section covered more advanced EC2 concepts that are tested in Solutions Architect scenarios, including public vs private vs Elastic IPs, placement groups, Elastic Network Interfaces (ENIs), and EC2 hibernation.

---

## Key Concepts Covered

- Public IP vs Private IP vs Elastic IP
- EC2 Placement Groups
- Elastic Network Interfaces (ENI)
- EC2 Hibernate
- scenario-based EC2 architecture details

---

## Key Takeaways

### Public vs Private vs Elastic IP
- Public IPs are reachable from the internet
- Private IPs are used for internal communication within a VPC
- Elastic IPs are static public IPv4 addresses that can be reassigned to resources

### Placement Groups
- Placement groups control how EC2 instances are placed on AWS infrastructure
- They are useful when workload communication or availability requirements matter
- Cluster Placement Groups are for high-performance, low-latency communication between instances

### Elastic Network Interfaces (ENI)
- ENIs are virtual network interfaces for EC2 instances
- ENIs belong to a subnet
- Because they belong to a subnet, they are tied to a specific Availability Zone
- ENIs can be detached and reattached within the same AZ

### EC2 Hibernate
- Hibernation preserves the contents of RAM by saving it to the root EBS volume
- Hibernate is useful when application state in memory needs to be resumed quickly
- Hibernate is different from stop because stop does not preserve RAM contents

---

## Main Review Items

### EC2 Hibernate
- when hibernation is supported
- how hibernation differs from stop and terminate
- when hibernation is useful in real scenarios

### Elastic Network Interfaces (ENI)
- ENIs are tied to a subnet and AZ
- ENIs cannot be attached across Availability Zones
- understand when a secondary ENI is useful

### EC2 Placement Groups
- Cluster Placement Group for low-latency / high-throughput workloads
- recognize HPC / big data / tightly-coupled workload clues
- distinguish placement group use cases from general EC2 scaling scenarios

---

## High-Yield Takeaways
- ENIs are scoped to a subnet and Availability Zone
- Hibernate preserves RAM state; stop does not
- Placement groups matter when EC2 instances must communicate at very high speed
- Cluster Placement Groups are common for HPC and big data compute clusters
- Specialized EC2 features often appear in scenario-heavy SAA questions

---

## Common Exam Traps
- confusing stop with hibernate
- assuming ENIs can be attached across AZs
- missing cluster placement group clues in high-throughput compute scenarios
- treating specialized EC2 features like generic EC2 behavior

---

## Quiz Result Reflection
I scored **2/5** on this section quiz. This section exposed real weak spots in advanced EC2 scenario handling, especially around **Hibernate**, **ENIs**, and **Placement Groups**.

---

## What I Need to Review Again
- Hibernate vs Stop vs Terminate
- ENI = subnet + AZ scoped
- Cluster Placement Group = low latency / high throughput / tightly-coupled compute
