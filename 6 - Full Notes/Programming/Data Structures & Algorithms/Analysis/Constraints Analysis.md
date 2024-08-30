
2024-08-30 16:09

Tags: [[Leetcode]] | [[Data Structures & Algorithms]] | [[Prep]]

### Overview
Read the problem constraints to determine the type of algorithm you should use, specifically the range of **input values**.

#### Example: Constraints - 1 <= x <= 10^5
This means input `x` is between 1 and 100,000 elements.

Based on this constraint, we can infer the time complexity our solution should have.

### Explanation
`n = 100,000`

Solution can be: `O(n)` or `O(n log n)` => between range [100,000, 500,000]

Solution cannot be: `O(N^2)` => 100,000^2 = 10,000,000,000 = 10^10 **in the worst case**

| Input Size | Time Complexity | Algo Solution |
| --------------- | --------------- | --------------- |
| n < 20 | 2^n or n! | Brute Force, [[Backtracking]] |
| n < 3000 | n^2 | [[Dynamic Programming]] |
| 3000 < n < 10^6 | O(n), O(n log n) | [[Sliding Window]], [[Greedy]], [[Heap]], [[Sorting]] |
| n > 10^6 | O(log n), O(1) | [[Binary Search]], Math |


### Source Material
- [Youtube Link](https://www.youtube.com/watch?v=eB7SMsE6qEc)

