
2024-09-11 17:58

Tags: [[Elixir]]

### Overview
Builds on [[GenStage]] and provides a higher-level abstraction for coordinating data processing pipelines in a more declarative way.

### Code
```elixir
{:ok, producer} = GenStage.start_link(MyProducer, initial_stage)
{:ok, consumer} = GenStage.start_link(MyConsumer, [])
```

### References
- [[Coordination Primitives]]

