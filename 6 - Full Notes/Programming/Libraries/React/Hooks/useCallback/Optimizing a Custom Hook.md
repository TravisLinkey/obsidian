
2024-09-13 16:54

Tags: [[React]]

### Overview
If you're writing a custom [[Hooks]], it's recommended to wrap any functions that it returns into `useCallback`.

This ensures consumers of your Hook can optimize their own code when needed.

### Code
```javascript
function useRouter() {
  const { dispatch } = useContext(RouterStateContext);

  const navigate = useCallback((url) => {
    dispatch({ type: 'navigate', url });
  }, [dispatch]);

  const goBack = useCallback(() => {
    dispatch({ type: 'back' });
  }, [dispatch]);

  return {
    navigate,
    goBack,
  };
}
```

### References
- [[useCallback]]
- [[Hooks]]

