Tags: [[AWS]] | [[Identity & Federation]]


### Overview
AWS Security Token Service is a web service that enables you to request temporary, limited-privilege credentials for users.

Allows you to assume [[Roles]] across different accounts, within the same accounts, and allows for identity federation.


### Use Cases

- Provide access for an [[IAM]] user in one AWS account that you own to access a [[Resources]] in another account that you own.
- Provide access to [[IAM]] users in AWS accounts owned by third parties.
- Provide access for services offered by AWS to AWS [[Resources]].
- Provide access for externally authenticated users ([[Identity Federation]]).

### Benefits

- Must *explicitly grant your users permission* to assume the role.
- You can add **multi-factor authentication** (MFA) protection to the role so that only users who sign in with an MFA device can assume the role.
- [[Principle of Least Privilege]] and it adds an auditing using [[CloudTrail]]

### References
- [[IAM]]
