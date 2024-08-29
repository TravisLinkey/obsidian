
2024-08-27 18:58

Tags: [[Rust]]

### Overview
Ensures memory safety without needing a garbage collector.

It enforces rules that prevent data races, dangling pointers, and invalid memory access.

### Key Concepts
1. [[Ownership]]
2. [[Borrowing]]
3. [[Rules Enforced]]
4. [[Lifetimes]]

### Key Points
- No double borrowing: You cannot have an immutable and a mutable reference to the same data simutaneously.

- Safety Guarantees: Borrow checker ensures memory safety and prevents data races at compile-time, meaning issues are caught early.

- Compile-Time Enforcement: Borrow checker works at compile-time, so you don't encounter these issues at runtime, resulting in fewer bugs.

- Lifetimes and scoping: [[Lifetimes]] play an essential role in managing how a reference remains valid, which is critical in avoiding dangling pointers.

### References
- [[Rust]]

