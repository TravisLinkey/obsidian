
2024-08-16 12:28

Tags: [[AWS]] | [[Identity & Federation]]

### Overview
Provides ongoing governance for your [[AWS Control Tower]] environment. (AWS Accounts)

### Two types
1. Preventative
    - using [[Service Control Policies]]
        - Ex. disallow creation of [[Access Keys]] for the root user.

2. Detective
    - using [[AWS Config]]
        - Ex. detect whether [[MFA]] for the root user is enabled.
        - Ex. monitor un-tagged resources creation, trigger [[SNS]] to alert admins.

### Three levels
1. Mandatory
    - Automatically enabled and enforced by [[AWS Control Tower]]
        - Ex. disallow public Read access to the Log Archive account

2. Strongly Recommended
    - Based on [[AWS Best Practices]] (optional)
        - Ex. enable encryptionh for [[EBS]] volumes attached to [[EC2]] instances.

3. Elective
    - Commonly used by enterprises (optional)
        - Ex. disallow delete actions without [[MFA]] in [[S3]] buckets

### References
- [[AWS Control Tower]]

