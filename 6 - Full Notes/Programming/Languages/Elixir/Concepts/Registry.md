
2024-09-11 17:58

Tags: [[Elixir]]

### Overview
A module which allows [[Processes]] to register themselves under a unique key.

This provides a way for processes to be looked up and communicated with by their registered name.

### Benefits
Allows processes to discover and communicate with each other easily based on names or types.

### Code
```elixir
{:ok, _} = Registry.start_link(keys: :unique, name: MyRegistry)
Registry.register(MyRegistry, :my_process, pid)
```

### References
- [[Coordination Primitives]]

