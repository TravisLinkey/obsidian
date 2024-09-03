
2024-09-02 17:32

Tags: [[System Design]] | [[AWS]]

### Overview
Fault tolerance with [[AWS]] [[MicroService]] architecture can be achieved with the use of [[DLQ]], [[Exponential Backoff]], and retries.

### Ensuring Fault Tolerance
1. [[At least once delivery]]
    - [[EventBridge]] guarantees at-least-once delivery of events.
    - [[Handling Duplicate Events]]
    - [[Exponential Backoff]]
        - EventBridge automatically retries event delivery in case of transient failures.
        - It uses exponential backoff which reduces the risk of overwhelming the downstream services that might be recovering from a failure.

### References
- [[Fault Tolerance]]

