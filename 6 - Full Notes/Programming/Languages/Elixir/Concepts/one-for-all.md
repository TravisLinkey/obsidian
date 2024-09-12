
2024-09-11 18:17

Tags: [[Elixir]]

### Overview
If a single child [[Processes]] crashes, all the child processes are terminated and restarted together.

The failure of one process affects all of the other child processes.

### Use Case
Used when the child processes are tightly coupled or dependent on each other.
- If one process's failure would make the other processes unstable or inconsistent, restarting all processes ensures that the system is in a consistent state.

### Diagramm
```css
Supervisor
├── A (all processes restart if any one crashes)
├── B (crashes, A and C are also terminated and restarted)
└── C
```

### References
- [[Supervisors]]
- [[Fault Tolerance]]


