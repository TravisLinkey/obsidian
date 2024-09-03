
2024-09-03 06:04

Tags: [[AWS]] | 

### Concepts
- [[KeyConditionExpression]]
- [[ExpressionAttributeValues]]

### Syntax
1. First initialize the `AWS SDK`
```javascript
const AWS = require('aws-sdk');

const dynamoDB = new AWS.DynamoDB.DocumentClient();
```

2. Define query parameters
```javascript
const params = {
  TableName: 'YourTableName',
  KeyConditionExpression: 'partitionKeyName = :partitionKeyValue',
  ExpressionAttributeValues: {
    ':partitionKeyValue': 'yourPartitionKeyValue',
  },
  // Optional parameters
  // FilterExpression: 'attributeName = :attributeValue',
  // ProjectionExpression: 'attribute1, attribute2',
};
```

3. Execute the query
```javascript
dynamoDB.query(params, (err, data) => {
  if (err) {
    console.error('Unable to query. Error:', JSON.stringify(err, null, 2));
  } else {
    console.log('Query succeeded:', JSON.stringify(data, null, 2));
  }
});
```

### References
- [[DynamoDB]]

