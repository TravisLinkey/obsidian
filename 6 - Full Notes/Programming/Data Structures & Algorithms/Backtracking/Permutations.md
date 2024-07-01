

2024-06-12 21:00

Tag: [[Data Structures & Algorithms]] | [[DFS]] | [[Backtracking]]

## Overview

Permutations can be though of as a decision tree where the first level of the tree contains each index of the array. Every layer we choose another index from the array from the elements that have not been chosen. Eventually we will end up with all permutations of the array.

To achieve this, we need to keep a list that represents whether a particular element has been used in the current branch or not. This can be done using [[DFS]] and [[Backtracking]]

### Code

```python
def permutations(nums):
	N = len(nums)

	used = [False] * N
	ans = []
	
	def dfs(current):
	
		if len(current) == N:
			ans.append(current[:])
			return
	
	for i in range(N):
		if not used[i]:
			used[i] = True
			current.append(nums[i])
			dfs(current)
			current.pop()
			used[i] = False
	  
	dfs([])
	return ans
```

## References:

[Leetcode Link]()