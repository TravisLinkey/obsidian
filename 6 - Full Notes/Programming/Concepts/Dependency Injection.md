
2024-09-02 16:11

Tags: [[]] | 

### Overview
When we pass the objects that a class needs, (the dependencies), instead of having it construct them itself.

This makes testing easy, because we can mock or stub out dependencies and test only the things we care about.

### Benefits
This also promotes decoupling and [[SOLID]] principles like the [[Open Closed Principle]] where we can carry along the needed dependencies, allowing our base classes to be easily extendable.

### References
- [[Open Closed Principle]]

