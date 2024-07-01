
2024-06-12 21:00

Tag: [[Data Structures & Algorithms]] | [[DFS]] | [[Backtracking]]

## Overview

The key to this algorithm is noticing that is a [[Backtracking]] algorithm. One obvious clue is the output will contain an empty list `[]` , and lists with only one element, `[1], [2], [3], ...` for each element in the array.

This means we will need to keep track of the current path, `current` and append it to the solutions array as a base case.

Additionally, we can see that we will also need to have a subset that contains all elements in the array, `[1, 2, 3, ...]` for each element in the array. This means we will need to have a `for` loop to iterate through each element, starting from the `0` index.

With these ideas in mind, we arrive at the [[Backtracking]] solution shown below.

### Code

```python
def subsets(self, nums: List[int]) -> List[List[int]]:
	N = len(nums)

	ans = []
	def backtrack(index, cur):
		ans.append(cur[:])
			
		for i in range(index, N):
			cur.append(nums[i])
			backtrack(i + 1, cur)
			cur.pop()

	backtrack(0, [])
	return ans
```

## References:

- [Leetcode Link](https://leetcode.com/problems/subsets/)

- [YouTube Link](https://www.youtube.com/watch?v=kSU-JY0_Bj8)