
2024-08-16 12:41

Tags: [[AWS]] | [[Identity & Federation]]

### Overview
Accounts can share VPC, including [[Private Subnet]].

### Details
- Each account is responsible for its own resources.
- Cannot view, modify or delete other resources in other accounts.

### Benefits
- Anything deployed in the VPC can talk to other resources in the VPC
- Applications are accessed easily across accounts, using **Private IP**!

### Use Cases
- Applications with the same trust boundaries.
- Applications with a high degree of interconnectivity.
- [[Managed Prefix List]]

### References
- [[AWS Resource Access Manager]]

