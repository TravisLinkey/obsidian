
2024-06-08 18:19

Tag: [[Database]]

## Overview

A set of properties of database transactions intended to guarantee data validity despite errors, power failures, and other mishaps.

A sequence of database operations that satisfies the ACID properties is called a *transaction.*

### Characteristics

1. ***Atomicity*** - A transaction either succeeds completely or fails completely.
2. ***Consistency*** - A transaction can only bring the database from one consistent state to another, preserving database invariants.
3. ***Isolation*** - Ensure concurrent execution of transactions leaves the database in the same state that would have been obtained if the transactions were executed sequentially.
4. ***Durability*** - Once a transaction has been committed, it will remain committed even in the case of a system failure.

## References:

[Wiki Link](https://en.wikipedia.org/wiki/ACID)
