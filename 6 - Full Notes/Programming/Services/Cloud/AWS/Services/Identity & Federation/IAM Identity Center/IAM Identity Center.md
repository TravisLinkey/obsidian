
2024-08-15 18:40

Tags:  [[AWS]] | [[Identity & Federation]] 

### Overview
Allows for Single Sign-On [[SSO]] for all:
    - AWS accounts (In [[AWS Organization]])
    - Business cloud applications (Salesforce, Box, Microsoft 365, etc)
    - [[SAML]] 2.0 enabled applications
    - [[EC2]] instances

### Details
Users for this SSO can be either:
    - Identity store in [[IAM Identity Center]]
    - Third party [[Active Directory]], OneLogin, Okta, etc...

### Key Concepts
- [[Permission Sets]] define what users have access to what.
    - Need to be associated with a specific [[OU]]
    - Need to be assigned to a `Group of Users`

- [[Attribute Based Access Control]]

### References
- [[Week 1]]

