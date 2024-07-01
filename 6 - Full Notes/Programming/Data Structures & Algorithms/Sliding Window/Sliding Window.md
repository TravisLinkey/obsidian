
2024-05-28 05:40

Status:
Tag: [[Data Structures & Algorithms]] | [[Array]]

# Sliding Window

This technique is used when you need to find sub-strings (contiguous sub-arrays) that satisfy some condition.

To do this, we use a left and right pointer and loop over the elements in the list, with right being the leading index. Each iteration, we add the right element to the sliding window (deque), and decide if we should shrink the size of the window based on some condition, or invariant.

If we need to shrink the window size, we move the left pointer forward, and recalculate our condition.

| Time Complexity |
| ------------- |
| O(N) |

### Related Techniques

This technique is used in more advanced algorithms like the [[MonoQueue]] 

### Problems

- [[1438. Longest Continuous Subarray With Absolute Diff Less Than or Equal to Limit]]
- [1208. Get Equal Substrings Within Budget](https://leetcode.com/problems/get-equal-substrings-within-budget/description/?envType=daily-question&envId=2024-05-28)
## References:

[Stack Overflow](https://stackoverflow.com/questions/8269916/what-is-sliding-window-algorithm-examples)
