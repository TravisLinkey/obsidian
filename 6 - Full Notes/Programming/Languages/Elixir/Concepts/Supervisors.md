

2024-09-11 17:58

Tags: [[Elixir]]

### Overview
[[Processes]] that monitor other processes, particularly in terms of [[Fault Tolerance]].

They ensure that if a child process crashes, it can be restarted according to a defined strategy ([[one-for-one]], [[one-for-all]]).

### Details
They are the foundation for `Supervision trees`, which are used extensively in [[Elixir]]applications to manage process lifecycles.

### Code
A simple supervisor setup:
```elixir
children = [
    {MyWorker, arg}
]
Supervisor.start_link(children, strategy: :one_for_one)
```

### References
- [[Concurrency Primitives]]

