
2024-06-09 17:04

Tag: [[Database]] | [[Optimization]] | [[3 - Tags/ADR|ADR]]

## Read Heavy Workloads

### [[SQL]]

1. [[MySQL]] / [[MariaDB]] with [[Read Replicas]]
- These databases can be configured to distribute read requests across multiple replicas, reducing the load on the primary database.

2. [[PostgreSQL]] with [[Read Replicas]]
- Overall throughput scales with the number of replicas.

3. [[SQLite]]
- Extremely low read latency, due to its in-process nature.
- Read throughput limited to a single process and the underlying storage performance.



### [[NoSQL]]

1. [[Cassandra]]
- A highly scalable database optimized for write-heavy workloads, but also performs well in read-heavy scenarios with its distributed architecture.

2. [[MongoDB]] with [[Sharding]] and [[Read Replicas]]
- These options can be configured to handle read operations efficiently.

3. [[Elasticsearch]]
- Optimized for searching and indexing large volumes of data quickly.


### Expected Read Latency

| Database | Read Latency (ms) | Read Throughput (w/s) |
| --------------- | --------------- | --------------- |
| MySQL / MariaDB | 1-5 | 1,000+ per replica  |
| PostgreSQL | 1-5 | 1,000+ per replica |
| SQLite | < 1 | 100-1000 |
| Cassandra | 5-15 | 10,000+ |
| MongoDB | 1-10 | 1,000-10,000+ |
| Elasticsearch | < 100 | 10,000+ |

