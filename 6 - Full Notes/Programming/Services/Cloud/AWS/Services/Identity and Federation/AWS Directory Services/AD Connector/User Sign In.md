
2024-08-15 10:47

Tags: [[Identity & Federation]] | [[AWS]] | [[Active Directory]] 

### Overview
For signing in using [[AD Connector]] to access [[AWS]] resouces On-Prem.

### Steps
1. User signs in with credentials (over [[SSL]])
2. Custom Sign-in page routes to [[AD Connector]]
3. [[AD Connector]] proxies request to On-Prem [[Active Directory]] to perform [[LDAP]] authentication.
4. Assume [[STS]] role for temporary credentials
5. Access [[AWS]] resources

### References
- [[AD Connector]]
