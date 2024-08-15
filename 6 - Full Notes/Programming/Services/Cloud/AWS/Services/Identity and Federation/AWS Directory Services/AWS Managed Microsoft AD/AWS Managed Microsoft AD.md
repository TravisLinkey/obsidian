
2024-08-07 19:47

Tags: [[AWS]] | [[Identity & Federation]] | [[Active Directory]] | [[AWS Managed Microsoft Managed AD]]

### Overview
A managed [[Active Directory]] solution by AWS.

### Purpose
To establish a 'trust' connection between your On-Prem AD and AWS

- Users are defined in two places, in AWS and On-Prem AD

**Suppports MFA**

### Details
- A Microsoft AD in your AWS [[VPC]]

### Capabilities
- [[EC2]] Windows instances can join the domain and run traditional AD applications (sharepoint, etc)

- Seamlessly [[Domain Join]] Amazon EC2 instances from multiple accounts and [[VPC]]s

- The most integrated with [[AWS]] offering from [[AWS Directory Services]]

### Deep Dive 
- [[Connect to On-Prem AD]]
- [[Active Directory Replication]]


### References
- [[AWS Directory Services]]

