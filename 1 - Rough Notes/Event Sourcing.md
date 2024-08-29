
2024-08-28 20:59

Tags: [[Architectural Pattern]]

### Overview
Where the state of an application is determined by a sequence of events rather than by storing the current state directly.

Each change is captured as an immutable event, and the current state can be reconstructed by replaying these events in the order they occured.

### Key Concept
- [[CQRS]] pattern

### Key Points
- [[Immutable Event]]
- [[State Reconstruction]]
- [[Auditability]] and [[Traceability]]
- Flexibility and Scalability
- Complexity and Storage

### References
- [[Mike Interview]]

