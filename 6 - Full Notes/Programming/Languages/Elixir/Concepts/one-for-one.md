
2024-09-11 18:17

Tags: [[Elixir]]

### Overview
If a child [[Processes]] crashes, only that specific process is restarted. 

The failure of one child does not affect the other child processes.

### Use Case
Most commonly used strategy because it is simple and it isolates failures to an individual process.

### Diagram
```css
Supervisor
├── A
├── B (crashes, only B is restarted)
└── C
```

### References
- [[Supervisors]]
- [[Fault Tolerance]]

