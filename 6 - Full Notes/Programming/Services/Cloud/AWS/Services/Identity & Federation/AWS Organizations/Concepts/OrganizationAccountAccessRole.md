
2024-08-15 11:14

Tags: [[AWS]] | [[Identity & Federation]]

### Overview
When we create a member account from the Organization Service API, the [[OrganizationAccountAccessRole]] is created automatically.

When administrative duties need to be performed on that member account, this role will be assumed.

### Details
This role grants full administrator permissions in the `Member` account to the `Management` account.

**If you invite an existing Member account, this role must be created manually**

### References
- [[AWS Organizations]]

