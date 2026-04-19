# Decision Notes

This file tracks high-value AWS service comparisons and architecture tradeoffs for SAA-C03.

## EC2 vs Lambda

### EC2
- Best when you need full OS-level control
- Useful for long-running workloads and custom environments

### Lambda
- Best for event-driven, short-duration, serverless execution
- Lower operational overhead for many use cases

### Common exam trap
Choosing EC2 when a serverless managed option is the better fit.

---

## IAM User vs IAM Role

### IAM User
- Used for a person or application needing long-term AWS access
- Can have console login and/or access keys

### IAM Role
- Used for temporary assumed permissions
- Best for AWS services, applications, and temporary access patterns

### Common exam trap
Choosing an IAM user where an AWS service should assume a role instead.

## EC2 Hibernate vs Stop vs Terminate

### Hibernate
- Saves the contents of RAM to the root EBS volume
- Useful when you want to resume an instance more quickly with application state preserved
- Best when preserving in-memory state matters

### Stop
- Instance shuts down, but attached EBS volumes can remain
- Does not preserve RAM contents
- Useful when you want to pause compute usage without deleting the instance

### Terminate
- Instance is deleted
- Used when the instance is no longer needed

### Common exam trap
Confusing hibernate with stop. Hibernate preserves RAM state; stop does not.
