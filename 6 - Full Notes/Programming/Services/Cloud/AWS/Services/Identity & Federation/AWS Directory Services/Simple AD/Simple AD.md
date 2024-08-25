
2024-08-07 19:57

Tags: [[Identity & Federation]] | [[AWS]] | [[Active Directory]]

### Overview
[[Active Directory]] compatible managed directory on AWS.

- Users are only defined on AWS

**Cannot be joined with on-prem AD**

### Use Cases
- Small: 500 users
- Large: 5000 users

### Benefits
- Inexpensive
- Low scale
- Basic AD or [[LDAP]] compatibility

### Capabilities
- Supports joining EC2 Instances, manage users and groups.

### Limitations
- No trust relationship
- Does not support [[MFA]], [[RDS]] [[SQL Server]], [[AWS]] [[SSO]]

### References
- [[AWS Directory Services]]
