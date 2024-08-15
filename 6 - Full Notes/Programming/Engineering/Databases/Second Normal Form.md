
Tags: [[Relational Database]]

## Second Normal Form = 2NF


### Overview

Rule: Ensure that all non-key columns are fully dependent on the [[Primary Key]]. This means eliminating partial dependencies where a non-key column is dependent on part of a [[Composite Primary Key]]

- Database must be in [[First Normal Form]]
- Non partial dependency - All non-prime attributes should be fully functionally dependent on the [[Candidate Key]]

#### Example: Split a table into two to separate the data that is dependent on only a part of the primary key.

-> Composite Key: (StudentId, Course)

| StudentId | Course | Instructor |
| --------------- | --------------- | --------------- |
| 1 | Math | Dr. Smith |
| 1 | Science | Dr. Smith |
| 2 | English | Dr. Green |

2NF:

| StudentId | Course  |
| --------- | ------- |
| 1         | Math    |
| 1         | Science |
| 2         | English |

| Course  | Instructor |
| ------- | ---------- |
| Math    | Dr. Smith  |
| Science | Dr. Brown  |
| English | Dr. Green  |

#### Details

Notice in our example above, Instructor has nothing to do with the StudentId, it only cares about the Course. This violates rule #2, Non partial dependency.

To fix this, we split up the Instructor, and pair it with the Course, and split up the StudentId and pair it with the Course.


### References
- [[Database Normalization]]

 [Youtube link](https://www.youtube.com/watch?v=J-drts33N8g)
