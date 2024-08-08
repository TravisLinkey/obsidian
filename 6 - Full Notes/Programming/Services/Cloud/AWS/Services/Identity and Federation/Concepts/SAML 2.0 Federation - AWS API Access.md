
2024-08-07 17:33

Tags: [[Identity Federation]] | [[SAML]] | [[AWS]] | [[STS]]

The user can access AWS Resources by providing a valid token from [[STS]]. This token will be issued to them once they call `AssumeRoleWithSAML` API using a valid [[SAML Assertion]] which was provided to them by their [[LDAP]] based identity store.


### References
- [[SAML]]

