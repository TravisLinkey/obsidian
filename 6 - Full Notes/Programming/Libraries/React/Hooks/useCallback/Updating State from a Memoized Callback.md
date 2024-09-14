
2024-09-13 16:54

Tags: [[React]]

### Overview
Sometimes you might need to update state based on previous state from a memoized callback.

### Example
This `handleAddTodo` function specifies `todos` as a dependency because it computes the next todos from it:

```javascript
function TodoList() {
  const [todos, setTodos] = useState([]);

  const handleAddTodo = useCallback((text) => {
    const newTodo = { id: nextId++, text };
    setTodos([...todos, newTodo]);
  }, [todos]);
  // ...
```

You want memoized functions to have as few dependencies as possible. You can remove that dependency by passing an `updater function` instead:

```javascript
function TodoList() {
  const [todos, setTodos] = useState([]);

  const handleAddTodo = useCallback((text) => {
    const newTodo = { id: nextId++, text };
    setTodos(todos => [...todos, newTodo]);
  }, []); // ✅ No need for the todos dependency
  // ...
```

### References
- [[useCallback]]
- [[Hooks]]

