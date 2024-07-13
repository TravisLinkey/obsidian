
Tags: [[STS]]

### Overview

The following steps must be taken to allow 3rd party access to [[Resources]] within your AWS account.

### Steps
1. Third party must have an AWS account ID.
2. Must create an `External Id` (a secret between you and the 3rd party).

    - To uniquely associate with the role between you and 3rd party.
    - Must be provided when defining the trust and when **assuming the role**.
    - Must be chosen by the 3rd party.

3. Define permissions in the [[IAM Policies]]


### References
- [[STS]]

