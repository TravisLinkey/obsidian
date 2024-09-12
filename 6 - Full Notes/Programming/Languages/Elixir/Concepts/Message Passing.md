
2024-09-11 17:58

Tags: [[Elixir]]

### Overview
[[Processes]] communicate via this mechanism.

Each process has a `mailbox`, where incoming messages are stored until the process is ready to handle them.

### Code
You can send a message to a process using the `send/2` function.
```elixir
send(pid, "Hello")
```

A process can retrieve a message from its mailbox using the `receive` block.
```elixir
receive do
    message -> IO.puts("Received: #{message}")
end
```

### References
- [[Concurrency Primitives]]

