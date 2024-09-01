
2024-08-31 11:07

### Overview
A concurrency model of [[Elixir]] where `Actors` are the fundamental units of computation.

In this model `Actors` communicate with each other through message passing.
kjk
### Details
1. Actors as processes
    - `Actors` are lightweight processes managed by the [[BEAM]]. They are not the same as operating system threads; they are more lightweight and run with [[Concurrency]].
    - Thousands or even millions of them can run simutaneously on a single machine.
    - They have their own state and do no share memory, preventing race conditions.

2. Message passing
    - Communication is asynchronous, when they send a message, they do not wait for a response before continuing execution.

### References
- [[Elixir]]

