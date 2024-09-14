
2024-09-12 19:38

Tags: [[React]]

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
- [[Updating Parent Component in a Transition]]
- [[Displaying a Pending Visual State During Transition]]

### Source Material
- [Youtube link](https://www.youtube.com/watch?v=1xjSQJWejZM)

### References
- [[Hooks]]

