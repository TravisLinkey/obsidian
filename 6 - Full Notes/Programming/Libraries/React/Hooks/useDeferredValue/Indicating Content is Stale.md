
2024-09-13 16:27

Tags: [[React]]

### Overview
When it is not obvious to the user that the query may be running, you can change the styling to indicate the results are still loading.

### Code
To make it obvious that the results list does not match the latest query, you can add a visual indication when the stale result list is displayed:
```javascript
<div style={{
  opacity: query !== deferredQuery ? 0.5 : 1,
}}>
  <SearchResults query={deferredQuery} />
</div>
```

### References
- [[useDeferredValue]]
- [[Hooks]]

