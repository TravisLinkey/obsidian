
2024-06-09 11:09

Tag: [[System Design]] | [[Streaming Service]]

## Overview

A messaging guarantee that ensures that every message sent by a producer will be delivered to the consumer at least one time. In other words, no messages are lost.


### Details
- [[AWS]] - Services like FIFO [[SQS]] and [[Kinesis Data Streams]] ensure "At least once delivery".
- [[GCP]] - Services like [[Google Cloud Pub-Sub]] provide this guarantee.


### Considerations
Consumers must be [[Idempotent]] to handle duplicate message deliveries without causing issues.

One way to achieve this is Consumers should track the last processed record to avoid reprocessing duplicates.

### References:
- [[Kinesis Data Streams]]
- [[SQS]]
- [[Google Cloud Pub-Sub]]
