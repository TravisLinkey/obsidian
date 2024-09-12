

2024-09-11 17:58

Tags: [[Elixir]]

### Overview
Higher-level abstractions built on top of [[Processes]], making it easier to perform background work or asynchronous operations.

### Details
The `Task` module provides functions like `Task.async/1` and `Task.await/1` to start tasks and wait for their results.

### Code
```elixir
task = Task.async(fn -> some_heavy_computation() end)
result = Task.await(task)
```

### References
- [[Concurrency Primitives]]

