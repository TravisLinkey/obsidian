
Tags: [[Data Structures & Algorithms]]

This technique can be used to create a mapping between some attribute (usually an array of attributes we are looping through) and an index. 

In some cases, we can use this lookup table to return an index that will act as a bridge to other arrays we may care about. 

#### Example: Three arrays: `healths`, `positions`, `directions`
Since our calculations are relying on one of these arrays, namely `positions`, we can use a [[Lookup Table]] to map the position -> index, and use this index in the other arrays `healths`, `directions`, without creating any tuples or data structures to relate all of these array values. 

By using this lookup table, we can perform operations on all of these arrays simply by using the index. 

### References
- [[2751. Robot Collisions]]

