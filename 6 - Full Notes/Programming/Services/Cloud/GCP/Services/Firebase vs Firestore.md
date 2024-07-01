
### Key Differences

| Label      | Firebase                                                                              | Firestore                                                                                             |
| ---------- | ------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| Data Model | JSON tree structure, simpler, but potentially harder to scale and manage complex data | Document and Collection model, more flexible and scalable for complex, hierarchical data structures   |
| Querying   | Limited querying capabilities, can be complex and inefficient with large datasets     | Advanced querying capabilities, including compound queries and indexing.                              |
| Scaling    | Challenging to scale due to its single-region setup and limited querying              | Designed to scale automatically across mutliple regions, providing better performance and scalability |

### Conclusion

[[Firebase]] is the broader platform offering various services to support app development, while [[Firestore]] is a specific NoSQL database within Firebase designed for more complex and scalable data storage.

[[Firestore]] generally offers more advanced features compared to the Realtime Database [[Firebase]], making it suitable for a wider range of applications.


### References

- [[Firestore]]
- [[Firebase]]