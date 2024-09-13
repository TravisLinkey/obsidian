
2024-09-12 19:38

Tags: [[React]] | 

### Overview
Allows updating the state without blocking the UI.

### Code
```javascript
const [isPending, startTransition] = useTransition();
```

### Details
- `isPending` flag tells you if there is a pending `Transition`.
- `startTransition` function lets you mark a state update as a `Transition`.

### Use Cases
- [[Non-Blocking Transition]]


### References
- [[]]

