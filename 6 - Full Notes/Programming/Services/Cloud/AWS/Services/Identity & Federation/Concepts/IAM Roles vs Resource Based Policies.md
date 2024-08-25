
Tags: [[IAM]] | 

- When you **assume a role** (user, application or service), you give up your original permissions and take permissions assigned to the role.

- When using a **resource-based policy**, the principal doesn't have to give up any permissions.


### Example
User in Account A needs to scan a DynamoDB table in Account A and dump it in an S3 bucket in Account B.

