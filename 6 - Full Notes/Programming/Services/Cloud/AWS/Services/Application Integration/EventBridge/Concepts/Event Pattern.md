
2024-09-02 17:19

Tags: [[AWS]] | [[Event Driven]] | [[MicroService]]

### Overview
Defines the data [[EventBridge]] uses to determine whether to send the event to the target.


#### Example
```json
{
  "source": ["ecommerce.orders"],
  "detail-type": ["OrderPlaced", "PaymentCompleted"],
  "detail": {
    "paymentStatus": ["PENDING", "COMPLETED"]
  }
}
```
- This example will filter events coming from 'ecommerce.orders' of the event type `OrderPlaced` or `PaymentComplete`. 
- the 'detail' section further filters the events by 'paymentStatus'

### References
- [[EventBridge]]

