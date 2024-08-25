
2024-08-16 14:06

Tags: [[AWS]] | [[Identity & Federation]]

### Overview
A set of one of more [[CIDR]] blocks

### Benefits
- Makes it easier to configure and maintain [[Security Group]] and [[Route Table]].

### Details
Customer-managed prefix list

- Set of [[CIDR]]s that you define and manage.
- Can be shared with other [[AWS]] accounts or [[AWS Organizations]].
- **Modify to update many [[Security Group]] at once.**

### Example - Prefix List - A
| CIDR Number | IP |
| -------------- | --------------- |
| CIDR 1 | 10.0.0.0/16 |
| CIDR 2 | 192.168.0.0/24 |
| CIDR 3 | 192.134.1.62/32 |

Lets say these [[CIDR]] blocks represent the internal company network.

We can reference these CIDR blocks using the `Prefix List` in a [[Shared VPC]] 

#### Ex. Account B
[[Security Group]] inbound rules:

| Protocol | Port | Source |
| --------------- | --------------- | --------------- |
| SSH | 22 | `Prefix List - A` |

### References
- [[AWS Resource Access Manager]]
