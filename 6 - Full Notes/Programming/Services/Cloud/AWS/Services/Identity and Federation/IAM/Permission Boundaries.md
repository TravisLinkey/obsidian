
Tags: [[IAM]] | 


### Overview

Advanced feature to use a managed policy to set the maximum permissions an IAM entity can get.

Supported for users and roles (not groups)

### Use Case

- Delegate responsibilities to non administrators within their permission boundaries. For example to create new IAM users.
- Allow developers to self-assign policies and manage their own permissions, while making sure they can't "escalate" their privileges.
- Useful to restrict ***one specific user*** (instead of a whole account using [[Organizations]] and [[SCP]])

#### Example: This will result in ***No Permissions***
| IAM Permission Boundary                                                                                                                                                                                                                                                                               | IAM Permission Through IAM Policy                                                                                                                                                                         |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| {<br>    "Version": "2012-10-17"<br>    "Statement": [<br>        {<br>            "Effect": "Allow",<br>            "Action": [<br>                "s3:*",<br>                "cloudwatch:*",<br>                "ec2:*"<br>            ],<br>            "Resource": "*"<br>        }<br>    ]<br>} | {<br>    "Version": "2012-10-17"<br>    "Statement": [<br>        {<br>            "Effect": "Allow",<br>            "Action": "iam:CreateUser"<br>            "Resource": "*"<br>        }<br>    ]<br>} |

### Explanation

The [[Permission Boundaries]] on the Left hand side only allows actions on [[S3]], [[CloudWatch]], [[EC2]], this will override the right hand side permissions for [[IAM]].

### References
- [[IAM]]

