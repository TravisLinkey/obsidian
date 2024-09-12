
2024-09-11 18:20

Tags: [[Elixir]]

### Overview
A simple abstraction for managing state in [[Elixir]]. 

Allows you to store and retrieve state in a seperate process, without having to directly handle the [[Message Passing]] and [[Processes]] management yourself.

### Use Case
They are useful when you need a shared, mutable state that is safe to access concurrently from multiple processes.

### Code
```elixir
{:ok, agent} = Agent.start(fn -> 0 end)
Agent.get(agent, fn state -> state end)
```

### References
- [[Concurrency Primitives]]

