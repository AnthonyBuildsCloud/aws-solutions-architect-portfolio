# Section 4 — IAM & AWS CLI

## Status
Completed

## Quiz Score
8/9

## Section Summary
This section covered the foundations of IAM, how permissions are structured in AWS, how users and groups are managed, how policies work, the purpose of MFA, programmatic access through the AWS CLI and SDK, CloudShell, IAM roles for AWS services, and IAM security tools and best practices.

---

## Key Concepts Covered

- IAM Users
- IAM Groups
- IAM Policies
- MFA
- AWS Access Keys
- AWS CLI
- AWS SDK
- AWS CloudShell
- IAM Roles
- IAM Security Tools
- IAM Best Practices

---

## Key Takeaways

### IAM Users
- IAM users represent people or applications that need AWS access
- Users can have console passwords and/or access keys
- Long-term access should be controlled carefully

### IAM Groups
- IAM groups are collections of IAM users
- Groups simplify permission management
- Groups can contain users, but not other groups

### IAM Policies
- IAM policies are JSON documents used to define permissions
- Policies contain one or more statements
- A statement commonly includes:
  - Effect
  - Action
  - Resource
  - optional Condition

### MFA
- MFA improves account security by requiring a second factor during login
- MFA is especially important for the root account and privileged users

### AWS Access Keys, CLI, and SDK
- Access keys provide programmatic access to AWS
- The AWS CLI is used to interact with AWS from the command line
- The AWS SDK is used by applications to interact with AWS services
- Access keys must be protected and should not be hardcoded into applications

### CloudShell
- AWS CloudShell provides browser-based shell access to AWS
- It is useful for quick AWS CLI work without local setup

### IAM Roles
- IAM roles are identities with permissions that are assumed temporarily
- Roles are commonly used by AWS services, applications, and federated identities
- Roles help avoid hardcoding long-term credentials

### IAM Security Tools
- IAM Credential Report helps review credential status across IAM users
- IAM Access Advisor shows which services were accessed and helps identify unused permissions

### IAM Best Practices
- Use least privilege
- Enable MFA
- Avoid using the root account for daily work
- Prefer IAM roles where possible
- Review permissions regularly

---

## Root Account Security

### Best Practices
- Do not use the root account for everyday AWS administration
- Enable MFA on the root account
- Protect root credentials carefully
- Use IAM users or roles for regular administration

---

## IAM Security Tools

### IAM Credential Report
- Provides an account-wide report of IAM user credential status
- Useful for checking:
  - password enabled or not
  - MFA enabled or not
  - access key presence
  - access key age
  - credential rotation details

### IAM Access Advisor
- Shows which services a user has permission to access
- Shows when those services were last accessed
- Useful for identifying unused permissions

---

## Main Review Item

### IAM Security Tools
- IAM Credential Report
- IAM Access Advisor
- how MFA fits into IAM account security
- distinguishing security auditing tools from general IAM best practices

---

## High-Yield Takeaways
- IAM groups contain users, not other groups
- Policies are JSON permission documents
- Roles are used for temporary assumed permissions
- Root account should be protected with MFA and rarely used
- IAM Credential Report and IAM Access Advisor are important IAM security tools
- Least privilege is a core AWS security principle

---

## Common Exam Traps
- confusing IAM users with IAM roles
- assuming groups can contain other groups
- using the root account for routine administration
- mixing up IAM Credential Report and IAM Access Advisor
- overusing long-term access keys when roles are the better design

---

## Quiz Result Reflection
I scored **8/9** on this section quiz. My main weak area was **IAM Security Tools**, especially distinguishing **IAM Credential Report** from **IAM Access Advisor** and understanding their role in IAM security review.

---

## What I Need to Review Again
- IAM Credential Report vs IAM Access Advisor
- IAM User vs IAM Role
- root account + MFA best practice
