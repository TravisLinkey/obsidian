
2024-06-04 05:10

Status:
Tag: [[Data Structures & Algorithms]] | [[Graph]] | [[Shortest Path]]

## Overview


An algorithm to find the [[Shortest Path]] to all other nodes from a single source node for a weighted graph. (Only positive weights)

## Code

```python
def shortestPath(edges, n, src):
	
	# create the adjacency list
	adj_list = collections.defaultdict(list)
	for u, v, weight in adj_list:
		adj_list[u].append((weight, v))

	paths = {}
	minHeap = [[0, src]]   # [cost, node]
	
	while minHeap:
		w1, n1 = heapq.heappop(minHeap)
		if n1 in shortest:
			continue
		shortest[n1] = w1

		for n2, w2 in adj_list[n1]:
			if n2 not in shortest:
				heapq.heappush(minHeap, [w1 + w2, n2])
	
	return shortest
```

## References:

[Neetcode Reference](https://neetcode.io/courses/advanced-algorithms/14)
