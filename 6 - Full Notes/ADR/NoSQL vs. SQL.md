
2024-06-08 14:22

Tag: [[System Design]] | [[Database]] | [[3 - Tags/ADR|ADR]]

## SQL over NoSQL

1. Structured Data with a Fixed Schema:

	- [[SQL]] databases like [[PostgreSQL]] or [[MySQL]] enforce schema constraints, ensuring data integrity and consistency.

2. Complex Queries and Transactions:

	- Applications requiring complex queries, multi-table joins, and transactions with [[ACID]] (Atomicity, Consistency, Isolation, Durability) properties, such as financial systems or e-commerce platforms, are better served by [[SQL]] databases.

3. Data Integrity and Constraints:

	- When data integrity is crucial, such as an inventory management system or healthcare database, need the enforcement of constraints like foreign keys, unique constraints, and check constraints. This is enforced at the database level, ensuring accuracy and reliability of data.

4. Standardized Query Language ([[SQL]]):

	- When the use of [[SQL]] is important for ease of maintenance, portability, and interoperability with other systems.


## NoSQL over SQL 

1. Handling Large Volumes of Unstructured or Semi-Structured Data:

	- Applications that deal with large amounts of [[Unstructured Data]], such as social media platforms, content management systems, or IoT data, benefit from [[NoSQL]] databases like [[MongoDB]] or [[Cassandra]]. These databases can store data in a flexible schema-less format.

2. Scalability Requirements:

	- If the application requires a horizontal scalability to handle a large number of read and write operations across [[Distributed Systems]], a [[NoSQL]] database like [[Cassandra]] or [[DynamoDB]] is ideal. NoSQL databases are designed to scale out by adding more servers, ensuring high availability and performance.

3. Flexible Schema:

	- When a data schema is expected to evolve frequently or is not well-defined upfront, a NoSQL database is ideal.

4. High Throughput and Low Latency:

	- Realtime applications such as online gaming, financial transaction systems, or real-time analytics platforms require high throughput with low latency. A good option for this would be [[Redis]], an in-memory key-value store, provide the necessary performance.

5. Event-Driven and Big Data Applications:

	- Applications involving big data processing, such as real-time analytics, log analysis, or event-driven architectures, are well suited for NoSQL databases. Systems like Apache [[Kafka]] for event streaming combined with a NoSQL database for storage can handle the high velocity and volume of data.

## Examples

| NoSQL | Use Case | Reason |
| --------------- | --------------- | --------------- |
|  | Social Media Platform | NoSQL databases can handle large volumes of unstructured data and provide horizontal scaling to manage high traffic. A Flexible schema allows for quick iteration and adaptation to new content types and features. |
|  | Real-Time Analytics | Processes and analyzes large streams of data generated from various sources, requiring high throughput and low latency. |
|  | Ecommerce Product Catalog | Dynamic product vatalog with varying attributes and hierarchical relationships, requiring quick updates and fast search capabilities. |

| SQL | Use Case                     | Reason                                                                                                                                                                                                                                      |
| --- | ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|     | [[ERP System]]               | Requires well-defined schema to manage complex relationships between different business entities. PostgreSQL or [[Oracle]] provide robust support for ACID transactions, ensuring data consistency and integrity across business processes. |
|     | [[CRM System]]               | SQL database facilitates the generation of detailed reports and support for complex joins and aggregations necessary for customer analytics                                                                                                 |
|     | Financial Management Systems | Data integrity and ability to enforce constraints to maintain ACID properties is crucial for accurate financial operations and compliance.                                                                                                  |

