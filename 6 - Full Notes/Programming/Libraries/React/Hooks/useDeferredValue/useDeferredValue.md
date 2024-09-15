
2024-09-13 16:00

Tags: [[React]]

### Overview
A hook that allows you to defer updating a part of the UI.

### Code
```javascript
import { useState, useDeferredValue } from 'react';

function SearchPage() {
  const [query, setQuery] = useState('');
  const deferredQuery = useDeferredValue(query);
  // ...
}
```

### Details
- During the initial render, the `deferredQuery` will be the same as `query`
- During updates, the `deferredQuery` will "lag behind" the latest `query`.

** React will first re-render without updating the deferred value, and then try to re-render with the newly received value in the background.

### Use Cases
- [[Fresh Content is Loading]]
- [[Indicating Content is Stale]]
- [[Deferring Re-Rendering a Part of UI]]

### Source Material
- [Youtube link](https://www.youtube.com/watch?v=yIpHTYo3PY0)

### References
- [[Hooks]]

