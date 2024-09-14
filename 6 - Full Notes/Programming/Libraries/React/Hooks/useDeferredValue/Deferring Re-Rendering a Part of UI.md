
2024-09-13 16:27

Tags: [[React]]

### Overview
Applying `useDeferredValue` can be useful when a part of your UI is slow to re-render, you can prevent it from blocking the rest of the UI.

### Code
```javascript
function App() {
  const [text, setText] = useState('');
  const deferredText = useDeferredValue(text);
  return (
    <>
      <input value={text} onChange={e => setText(e.target.value)} />
      <SlowList text={deferredText} />
    </>
  );
}
```

### Explanation
Here `useDeferredValue` lets you prioritize updating the input (which must be fast) over updating the result list (which can be slower).

It tells React that re-rendering the list can be deprioritized so that it doesn't block the keystrokes. The list will "lag behind" the input and then "catch up", but will not block the user from typing.

### References
- [[useDeferredValue]]
- [[Hooks]]

