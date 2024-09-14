
2024-09-13 15:36

Tags: [[React]]

### Overview
You can update a parent component's state from the `useTransition` call.

### Code
This `TabButton` component wraps its `onClick` logic in a `Transition`:

```javascript
import { useTransition } from 'react';

export default function TabButton({ children, isActive, onClick }) {
  const [isPending, startTransition] = useTransition();
  if (isActive) {
    return <b>{children}</b>
  }
  return (
    <button onClick={() => {
      startTransition(() => {
        onClick();
      });
    }}>
      {children}
    </button>
  );
```

### Explanation
Because the parent component updates its state inside the `onClick` event handler, that state update gets marked as a `Transition` allowing us to immediately click other compoents without blocking.

### References
- [[useTransition]]
- [[Hooks]]

