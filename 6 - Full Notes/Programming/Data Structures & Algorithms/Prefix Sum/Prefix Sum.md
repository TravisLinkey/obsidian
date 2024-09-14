
2024-09-13 15:15

Tags: [[Data Structures & Algorithms]]

### Overview
A [[Prefix Sum]] can be used to efficiently calculate the sum over any subarray. 

### Details
To compute the sum of elements between indices `left` and `right`, we use the following formula:

$$
\sum_{i=\text{left}}^{\text{right}} A[i] = \text{prefix\_sum}[\text{right}] - \text{prefix\_sum}[\text{left} - 1]
$$

If `left = 0`, the formula simplifies to:

$$
\sum_{i=0}^{\text{right}} A[i] = \text{prefix\_sum}[\text{right}]
$$

### Example:

Let $A = [2, 4, 6, 8, 10]$ and the corresponding prefix sum array be:

$$
\text{prefix\_sum} = [2, 6, 12, 20, 30]
$$

To find the sum of elements between indices `left = 1` and `right = 3`:

$$
\sum_{i=1}^{3} A[i] = \text{prefix\_sum}[3] - \text{prefix\_sum}[0] = 20 - 2 = 18
$$

### References
- [[1310. XOR Queries of a Subarray]]

