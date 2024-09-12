

2024-09-11 17:58

Tags: [[Elixir]]

### Overview
Allow one [[Processes]] to watch another and be notified if the monitored process terminates.

Unlike [[Links]], monitors are unidirectional, meaning if the monitored process crashes, the monitoring process is notified but it does not crash.

### Code
You can setup monitoring with `Process.monitor/1`

```elixir
ref = Process.monitor(pid)
```

### References
- [[Concurrency Primitives]]

