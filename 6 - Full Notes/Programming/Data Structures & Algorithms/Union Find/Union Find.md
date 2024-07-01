
Tags: [[Data Structures & Algorithms]] | [[Minimum Spanning Tree]]


### Overview
This can be used to store a collection of disjoint (non-overlapping) sets.


### Implementation

```python
class UnionFind:
    def __init__(self, N):
        self.N = N
        self.parents = [x for x in range(N)]

    def ufind(self, x):
        if self.parents[x] != x:
            self.parents[x] = self.ufind(self.parents[x])
        return self.parents[x]

    def uunion(self, a, b):
        ua = self.ufind(a)
        ub = self.ufind(b)

        self.parents[ua] = ub

    def is_connected(self, a, b):
        return self.ufind(a) == self.ufind(b)
```

### References
[Wiki Link](https://en.wikipedia.org/wiki/Disjoint-set_data_structure)
