
2024-08-28 20:42

### Overview
AKA, `Native Implemented Function` or `NIF`

This is a function that is written in another language other than the source language and is executed within a virtual environment.

#### Example
[[Elixir]] has support for [[Native Function]], which means you can write [[C]] or [[Rust]] code and execute it within the [[Erlang Virtual Machine]].

### Benefits
- Used when you need to perform operations that are computationally intensive or require access to system-level resources not easily accessible from the source language.

- They can be significantly faster than the equivalent code in the source language.

### Considerations
- If there is a bug in the Native Function, (ex. a segmentation fault in C), it can crash the entire Virtual Machine or even your whole system.

- A primary risk of using NIF code is if it takes too long to execute, it can block the scheduler of the VM.

### References
- [[Erlang Virtual Machine]]
- [[Elixir]]
