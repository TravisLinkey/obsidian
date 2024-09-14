
2024-09-13 16:27

Tags: [[React]]

### Overview
A common alternative UI pattern is to **defer** updating the list of results and to keep showing previous result until the new results are ready. 

### Code
Call `useDeferredValue` to pass a deferred version of the query down:
```javascript
export default function App() {
  const [query, setQuery] = useState('');
  const deferredQuery = useDeferredValue(query);
  return (
    <>
      <label>
        Search albums:
        <input value={query} onChange={e => setQuery(e.target.value)} />
      </label>
      <Suspense fallback={<h2>Loading...</h2>}>
        <SearchResults query={deferredQuery} />
      </Suspense>
    </>
  );
}
```

### Explanation
The `query` will update immediately, so the input will display the new value. However, the `deferredQuery` will keep the previous value until the data has loaded, so `SearchResults` will show the stale results for a bit.

### References
- [[useDeferredValue]]
- [[Hooks]]

