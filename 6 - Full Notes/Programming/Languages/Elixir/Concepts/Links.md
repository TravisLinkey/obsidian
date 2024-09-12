

2024-09-11 17:58

Tags: [[Elixir]]

### Overview
A way to connect [[Processes]] such that if one process crashes, the linked process also crashes.

This is useful for managing process failures and ensuring that related processes either succeed or fail together.

### Code
You can link processes using the `Process.link/1` function.

```elixir
ref = Process.link(pid)
```

### References
- [[Concurrency Primitives]]
- [[Monitors]]

