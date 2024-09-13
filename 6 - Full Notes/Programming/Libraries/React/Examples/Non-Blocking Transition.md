
2024-09-12 19:47

Tags: [[React]]

### Overview
Call [[useTransition]] at the top level of your component to mark state updates as non-blocking `Transitions`.

### Example
- Keep the interface updates responsive even on slow devices
    ex. The user clicks a tab but then change their mind and click another tab, they can do that without waiting for the first re-render to finish.

### Code
```javascript
function TabContainer() {
  const [isPending, startTransition] = useTransition();
  const [tab, setTab] = useState('about');

  function selectTab(nextTab) {
    startTransition(() => {
      setTab(nextTab);
    });
  }
  // ...
}
```

### References
- [[useTransition]]

