
2024-08-10 22:03

Tags: [[JavaScript]]

### Overview
To sort a dictionary by key in [[JavaScript]] you need to use the `.sort()` method on the entries of the dictionary.

You can get the entries of a dictionary using the `Object.entries`.

The `.sort()` method returns an array of sorted `tuples`. You can convert this back to a dictionary using the `Object.fromEntries()` method.

### Details
This is demonstrated below with dictionary keys that are of the type `string` that represent dates.

### Code 
```javascript
let dictionary = {
    "2024-08-10": ["John", "Jane"],
    "2024-07-15": ["Alice", "Bob"],
    "2024-08-05": ["Charlie", "Dana"],
};

const sortedEntries = Object.entries(dictionary).sort((a, b) => {
    return new Date(a[0]) - new Date(b[0]);
})

console.log(sortedEntries);
// [["2024-07-15", ["Alice", "Bob"]], ["2024-08-05", ["Charlie", "Dana"]], ["2024-08-10", ["John", "Jane"]]]

const sortedDictionary = Object.fromEntries(sortedEntries);

console.log(sortedDictionary);
// {
//   2024-07-15: ["Alice", "Bob"],
//   2024-08-05: ["Charlie", "Dana"],
//   2024-08-10: ["John", "Jane"]
// }

```
