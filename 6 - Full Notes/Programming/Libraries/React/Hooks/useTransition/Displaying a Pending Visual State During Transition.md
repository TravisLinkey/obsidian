

2024-09-13 15:28

Tags: [[React]]

### Overview
The `isPending` boolean value returned by the [[useTransition]] can be used to indicate to the user that a Transition is in progress.

### Code
For example, the tab button can have a special "pending" visual state:
```javascript
import { useTransition } from 'react';

export default function TabButton({ children, isActive, onClick }) {
  const [isPending, startTransition] = useTransition();
  if (isActive) {
    return <b>{children}</b>
  }
  if (isPending) {
    return <b className="pending">{children}</b>;
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
}
```

### Explanation
Now clicking other tabs feels more responsive because we will use the special `className="pending"` to display special styles while the transition is pending.

### References
- [[useTransition]]
- [[Hooks]]

