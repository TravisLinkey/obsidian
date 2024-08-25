
2024-08-25 13:35

Tags: [[System Design]]

### Overview
Concurrency and parallelism are two distinct but related concepts.

#### Concurrency
The tasks are executed in overlapping time periods. They may not run at the exact same time, but their execution is interleaved.

Time:  |  1  |  2  |  3  |  4  |  5  |  6  |  7  |  8  |  9  | 10 |
       -----------------------------------------------------------
Task A |  A1 | A2 |    | A3 |    | A4 |    | A5 |    | A6 |
Task B |     |    | B1 |    | B2 |    | B3 |    | B4 |    |
       -----------------------------------------------------------

#### Parallelism
When two tasks are executed simutaneously. This process requires multiple processors or cores.

Time:  |  1  |  2  |  3  |  4  |  5  |  6  |  7  |  8  |  9  | 10 |
       -----------------------------------------------------------
Task A |  A1 | A2 | A3 | A4 | A5 | A6 |    |    |    |    |
Task B |  B1 | B2 | B3 | B4 | B5 | B6 |    |    |    |    |
       -----------------------------------------------------------

### Summary


### References
- [[]]

