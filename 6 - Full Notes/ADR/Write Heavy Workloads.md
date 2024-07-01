
2024-06-09 17:04

Tag: [[Database]] | [[Optimization]] | [[3 - Tags/ADR|ADR]]

## Write Heavy Workloads

### [[SQL]]

1. [[MySQL]] / [[MariaDB]] with Write-Optimized configuration
- Optimizing configurations like InnoDB settings to help increase write heavy workloads.
- Using partitioning and indexing strategies can also help.

2. [[PostgreSQL]] with Write-Optimized configuration


### [[NoSQL]]

1. [[Cassandra]]
- This database uses clustering which is ideal for write-heavy applications.

2. [[MongoDB]] with [[Sharding]]
- Write operations can be distributed across multiple shards, enhancing write performance.

3. [[DynamoDB]]
- This database is optimized for high write throughput and low latency


### Expected Write Latency

| Database | Write Latency (ms) | Write Throughput (w/s) |
| --------------- | --------------- | --------------- |
| MySQL / MariaDB | 1-10 | 1000+  |
| PostgreSQL | 1-10 | 1000+ |
| Cassandra | 1-10 | 10,000+ |
| MongoDB | 1-10 | 1,000-10,000 |
| DynamoDB | 1-10 | 100,000+ |

