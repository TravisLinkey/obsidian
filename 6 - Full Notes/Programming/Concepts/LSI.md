
2024-05-30 17:21

Status:
Tag: [[NoSQL]] | [[Database]]

## Overview

An index that has the same partition key as the base table, but with a different sort key.

It is "local" in the sense that every partition of a local secondary index is scoped to a base table partition that has the same partition key value.

## Details

- As a result of the shared scope (with base table partition with same pk value), the total size of the indexed items for any one partition key value can't exceed 10 GB.
- Shares provisioned throughput settings for read and write activity with the table it is indexing.
- By default, the **maximum number of LSI** per [[DynamoDB]] table is 5.
## References:

