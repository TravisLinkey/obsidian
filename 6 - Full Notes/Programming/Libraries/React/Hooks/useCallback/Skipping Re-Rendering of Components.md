
2024-09-13 16:54

Tags: [[React]]

### Overview

### Code
To cache a function between re-renders of your component, wrap its definition into the [[useCallback]] hook:


```javascript
function ProductPage({ productId, referrer, theme }) {
  // Tell React to cache your function between re-renders...
  const handleSubmit = useCallback((orderDetails) => {
    post('/product/' + productId + '/buy', {
      referrer,
      orderDetails,
    });
  }, [productId, referrer]); // ...so as long as these dependencies don't change...

  return (
    <div className={theme}>
      {/* ...ShippingForm will receive the same props and can skip re-rendering */}
      <ShippingForm onSubmit={handleSubmit} />
    </div>
  );
}
```
### Explanation
By wrapping `handleSubmit` in [[useCallback]], you ensure it's the same function between the re-renders. (until dependencies change)

### References
- [[useCallback]]
- [[Hooks]]

