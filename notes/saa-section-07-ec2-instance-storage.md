# Section 7 — EC2 Instance Storage

## Status
Completed

## Quiz Score
7/9

## Section Summary
This section covered EC2 instance storage concepts, including EBS, EBS snapshots, AMIs, instance store, EBS Multi-Attach, EBS encryption, EFS, and the comparison between EBS and EFS.

---

## Key Concepts Covered

- EBS Overview
- EBS Snapshots
- AMIs
- Instance Store
- EBS Volume Types
- EBS Multi-Attach
- EBS Encryption
- Amazon EFS
- EFS vs EBS

---

## Key Takeaways

### EBS Overview
- Amazon EBS provides block storage for EC2 instances
- EBS volumes are persistent
- EBS is commonly used for boot volumes and attached data volumes

### EBS Snapshots
- Snapshots are backups of EBS volumes
- Snapshots can be used to restore data or create new volumes
- Snapshots are useful for backup and recovery workflows

### AMIs
- AMIs are templates used to launch EC2 instances
- AMIs are Region-scoped
- AMIs can be copied across Regions when needed

### Instance Store
- Instance store provides local storage attached to the EC2 host
- It is useful for temporary data such as caches, buffers, or scratch data
- Data is lost if the instance stops or terminates

### EBS Volume Types
- Different EBS volume types fit different workloads
- High-performance databases may need higher-performance SSD options
- Volume choice should match performance and cost requirements

### EBS Multi-Attach
- EBS Multi-Attach allows specific EBS volumes to be attached to multiple EC2 instances
- This is a specialized feature and not the normal default pattern

### EBS Encryption
- EBS volumes can be encrypted for data-at-rest protection
- Encryption is an important storage security feature

### EFS vs EBS
- EBS is block storage for EC2
- EFS is shared file storage
- EFS is better when multiple instances need access to the same file system

---

## Main Review Items

### High-performance EBS volume selection
- recognize when a workload needs high IOPS
- know when Provisioned IOPS SSD volumes are the better fit
- distinguish performance-focused storage questions from general-purpose storage questions

### EBS volume behavior on EC2 instances
- root volume vs additional attached EBS volumes
- what happens to volumes on instance termination
- default delete-on-termination behavior for root volumes vs non-root volumes

---

## High-Yield Takeaways
- EBS is persistent block storage for EC2
- instance store is high-performance temporary local storage
- AMIs are Region-scoped
- high-IOPS database workloads often point toward Provisioned IOPS SSD volumes
- root and additional EBS volumes may behave differently on termination
- EBS and EFS solve different storage problems

---

## Common Exam Traps
- choosing the wrong EBS volume type for high-IOPS database workloads
- forgetting that root and non-root EBS volumes can behave differently on termination
- confusing EBS persistence with instance store temporary storage
- choosing EFS when the question is really about block storage

---

## Quiz Result Reflection
I scored **7/9** on this section quiz. My main weak areas were **high-performance EBS volume selection** and **root vs additional EBS volume behavior**.

---

## What I Need to Review Again
- high-performance EBS volume selection
- root volume vs non-root volume behavior
- instance store vs EBS persistence
- EBS Multi-Attach use cases
