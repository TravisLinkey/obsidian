
Tags: [[Relational Database]]

## Third Normal Form = 3NF


### Overview

Rule: Ensure that all non-key columns are fully dependent on the [[Primary Key]]. This means eliminating partial dependencies where a non-key column is dependent on part of a [[Composite Primary Key]].

- Database must be in the [[First Normal Form]] & [[Second Normal Form]]
- No transitive dependency - All fields must only be determinable by the primary/composite key, not by other keys.

#### Example: Split a table into two to separate data that is dependent on only a part of the primary key.

| StudentId | Course | Instructor | InstructorOffice |
| --------------- | --------------- | --------------- | --------------- |
| 1 | Math | Dr. Smith | Room 101 |
| 1 | Science | Dr. Brown | Room 102 |
| 2 | English | Dr. Green | Room 103 |

**3NF:**

| StudentId | Course |
| -------------- | --------------- |
| 1 | Math |
| 1 | Science |
| 2 | English |

| Course  | Instructor |
| ------- | ---------- |
| Math    | Dr. Smith  |
| Science | Dr. Brown  |
| English | Dr. Green  |

| Instructor | InstructorOffice |
| -------------- | --------------- |
| Dr. Smith | Room 101 |
| Dr. Brown | Room 102 |
| Dr. Green | Room 103 |

#### Explanation
The transitive dependency that needed to be removed is the dependency between `InstructorOffice` and `Instructor`.

A transitive dependency occurs when a non-key column depends on another non-key column, which in turn depends on the [[Primary Key]]. In this case, `InstructorOffice` depends on `Instructor` which depends on `Course`. Therefore, `InstructorOffice` is transitively dependent on `Course` through the `Instructor`.


### References
- [[Database Normalization]]

 [Youtube link](https://www.youtube.com/watch?v=J-drts33N8g)
