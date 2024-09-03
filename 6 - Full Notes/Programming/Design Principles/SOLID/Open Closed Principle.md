
2024-09-02 15:56

Tag: [[Design Principles]]

### Overview
Software Entities (classes, modules, functions, etc.) should be **open for extension but closed for modification**.

### Explanation:
This means you should be able to add *new functionality* to existing code **without changing the existing code**.

### Motivation:
The goal is to minimize the risk of introducing bugs into previously tested code while allowing the software to evolve and adapt to new requirements.

### Example:
Instead of modifying a class directly to add new functionality, you could use inheritance, [[Dependency Injection]] or composition to extend the class and add the new behavior.


### References
- [[SOLID]]

