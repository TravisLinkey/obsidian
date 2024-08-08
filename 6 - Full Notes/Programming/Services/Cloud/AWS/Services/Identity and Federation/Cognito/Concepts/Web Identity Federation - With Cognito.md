
2024-08-07 18:01

Tags: [[Identity Federation]] | [[AWS]] | [[STS]] | [[Cognito]]

This method is preferred over [[Web Identity Federation - Without Cognito]].

### Overview
A [[Cognito Token]] is used to retreive temporary security credentials from [[STS]]. This can be used to access AWS resources. A user must first sign into an [[IDP]] client side, to receive the ID Token to send to [[Cognito]].

### Steps
1. Login with [[IDP]]
2. ID Token issued
3. ID Token used to call [[Cognito]]
4. [[Cognito Token]] issued
5. Use [[Cognito Token]] to call [[STS]]
6. Temporary security credentials issued by [[STS]]
7. Access AWS resources

### Benefits
- Supports anonymous users
- Supports [[MFA]]
- Data Synchronization

### References
- [[Week 1]]

