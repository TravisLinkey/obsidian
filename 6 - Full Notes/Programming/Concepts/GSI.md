
2024-05-30 17:21

Status:
Tag: [[NoSQL]] | [[Database]]

## Overview

A global secondary index contains a selection of attributes from the base table, but they are organized by a primary key that is different from that of the table.

The index key does not need to have any of the key attributes from the table. It doesn't even need to have the same key schema as the table.

## Details

- GSI has its own provisioned throughput settings for read and write activity that is separate from the base table.
- By default, the **maximum number of GSI** per [[DynamoDB]] table is 20.

## References:

[AWS Docs](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/GSI.html#:~:text=A%20global%20secondary%20index%20contains,key%20schema%20as%20a%20table.)
[AWS Guidelines](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/bp-indexes-general.html)