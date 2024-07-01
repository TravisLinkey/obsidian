
2024-06-06 16:46

Status:
Tag: [[System Design]]

## Key Concepts:
- [[Geocoding]]
- [[Spatial Indexing]]
- [[Quadtree]]
### Business Requirements:
- Route from some source to some destination
- Track the users location
- Give estimated time of arrival (ETA)
- Also give information about traffic (heavy / light traffic, etc
#### Assumptions:
- We already have map data

### Non Functional Requirements:
- 1 Billion daily active users (DAU), Scale
- Accuracy
- Availability, reliability
- Latency is tolerated (~5 seconds)

### Deep Dive Solution:

[[Design Google Maps]]

## References:

[Neetcode IO](https://neetcode.io/courses/system-design-interview/7)