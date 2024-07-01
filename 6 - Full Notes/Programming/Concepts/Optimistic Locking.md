
Tags: [[Database]] | [[DynamoDB]] | [[Concurrency]]

A technique to handle concurrent updates by using a version number to ensure that updates do not overwrite each other.

Each record has an attribute that acts as a version number. If you retrieve an item from a table, the application records the version number of that item.

You can only update an item if the version number on the server side has not changed. If there is a version mismatch, it means the item was modified and you need to retrieve the item again and attempt the update.

### References
[AWS Docs](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBMapper.OptimisticLocking.html)