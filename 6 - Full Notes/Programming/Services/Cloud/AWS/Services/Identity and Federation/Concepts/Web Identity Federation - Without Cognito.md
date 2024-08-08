
2024-08-07 18:01

Tags: [[Identity Federation]] | [[AWS]] | [[STS]]

Access [[AWS]] resouces using temporary security credentials issued by [[STS]].

To get the creds, you must call the `AssumeRoleWithWebIdentity` API from a Client to begin the login process via an [[IDP]] (Identity Provider) such as Google, Facebook, Amazon, etc. 

After successful login, a `Web Identity Token` is issued and used to call the `AssumeRoleWithWebIdentity` API.

### Steps
1. Login with [[IDP]]
2. Web Token issued
3. Call `AssumeRoleWithWebIdentity` API
4. [[STS]] issues temporary security creds
5. Access AWS resources


### References
- [[Week 1]]

