
2024-08-07 19:52

Tags: [[Identity & Federation]] | [[AWS]] | [[Active Directory]]

### Overview
A `Directory Gateway` (proxy) to redirect to on-prem AD

### Purpose
Allow for users defined on-prem to connect to AWS.

Users are only defined on-prem. (Not in AWS)

**Supports MFA**

### Limitations 
- No caching capability
- No possibility of establishing a trust relationship
- Does not work with [[SQL Server]]
- Does not have seamless joining
- Cannot share directory

### Requirement
**Must have [[VPN]] or [[Direct Connect]] setup.**

### Deep Dive
- [[User Sign In]]

### References
- [[AWS Directory Services]]

