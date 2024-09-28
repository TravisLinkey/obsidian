2024-09-28 12:30

Tags: [[Python]]

### Overview

The `bisect_left(list, x)` function performs a [[Binary Search]] on the `list` and returns the index that the element `x` should be placed.

This performs an optimal search on a list and returns the index where the element can be placed. (Left index)

### Cases

#### Exists in array:

- If `x` is found in the `list`, it return the 0-indexed position of the elemnt.

#### Case too hight:

- If `x` does not exist in the list (too low), `bisect_left` returns a 0.

#### Case too high:

- If `x` does not exist in the list (too large), `bisect_left` returns the length of the list.

### Code

```python
import bisect

li = [1, 2, 4, 4, 4, 5, 8]

index = bisect.bisect_left(li, 4)
print("Found in list ", index) # returns 2

index = bisect.bisect_left(li, -2)
print("Not in list low: ", index) # returns 0

index = bisect.bisect_left(li, 10)
print("Not in list low high: ", index) # returns 5

```

### References
- [[My Calendar 1]]
