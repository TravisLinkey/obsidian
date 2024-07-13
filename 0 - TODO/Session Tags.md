
Tags: [[AWS]] | [[IAM]]

Tags that you pass when you assume an [[IAM Roles]] or federate user in [[STS]]

- `aws:PrincipalTag` Condition:
    - Compares the tag attached to the [[Principal]] making the request with the tag you specified in the policy

#### Example: allow a principal to pass session tags only if the principal making the request has the spcified tags

```json
{
  "Version": "2012-10-17",
  "Statement": {
    "Effect": "Allow",
    "Action": "s3:GetObject",
    "Resource": "arn:aws:s3:::example_bucket",
    "Condition": {
            "StringEquals": {
                "aws:PrincipalTag/Department": "HR"
            }
        }
  }
}
```


### References
- [[STS]]

