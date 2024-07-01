
2024-06-09 14:39

Tag: [[System Design]] | [[DynamoDB]] | [[Concurrency]]

## Overview

Due to the nature of our application, process financial transactions, and the design of our system, DynamoDB is massively scalable, we needed a way to ensure that concurrent updates to Dynamo records would not create inconsistent, unreliable data.

## Solution
- Use [[Optimistic Locking]] and [[Conditional Writes]]

### Conclusion

Before an update to a record could be made, we would compare a version number in the request being made to the version number of the record in the database. If there was a mismatch, we would need to pull the updated record and try the request again.

