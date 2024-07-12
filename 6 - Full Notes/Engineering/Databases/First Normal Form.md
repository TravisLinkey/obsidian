
Tags: [[Relational Database]] 

## First Normal Form = 1NF


### Overview

Rule: Ensure that each table has a [[Primary Key]] and that each column contains only atomic (indivisible) values. There should be no repeating groups or arrays.

- All rows must be unique (no duplicate rows)
- Each cell must only contain a single value (not a list)
- Each value should be non divisible (can't be split down further)

#### Example: Convert a table with multiple values in a single column into multiple rows.

| StudentId | Name | Courses |
| --------------- | --------------- | --------------- |
| 1 | Alice | Math, Science |
| 2 | Bob | English |

1NF:

| StudentId | Name | Courses |
| --------------- | --------------- | --------------- |
| 1 | Alice | Math |
| 1 | Alice | Science |
| 2 | Bob | English |


### References
- [[Database Normalization]]

 [Youtube link](https://www.youtube.com/watch?v=J-drts33N8g)

