
2024-09-11 17:58

Tags: [[Elixir]]

### Overview
Lightweight, isolated units of concurrency.

Not operating system threads but are managed by the [[BEAM]].

### Details
- Processes are extremely efficient, allowing millions to run concurrently on a single machine.
- **Isolated** so they do not share memory.
- All communication done via [[Message Passing]]

### Code
You can create a new process using the `spawn/1` function:
```elixir
spawn(fn -> IO.puts("Hello from a new process!") end)
```

### References
- [[Concurrency Primitives]]

