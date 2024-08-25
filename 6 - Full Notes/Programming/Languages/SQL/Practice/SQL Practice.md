2024-07-27 07:04

Tags: [[SQL]] | [[Interview]] | [[Practice]]

#### Question 1: Given the following tables, write a query to get the total number of orders placed by each customer, along with the customer's name. The output should be sorted by the total number of orders in descending order.

Orders:

| OrderId | CustomerId | OrderDate |
| --------------- | --------------- | --------------- |
| 1 | 1 | 2023-07-01 |
| 2 | 2 | 2023-07-02 |
| 3 | 1 | 2023-07-03 |
| 4 | 3 | 2023-07-04 |

Customers:

| CustomerId | CustomerName |
| -------------- | --------------- |
| 1 | Alice |
| 2 | Bob |
| 3 | Charlie |

```sql
SELECT c.CustomerName, COUNT(o.OrderId) AS TotalOrders
FROM Customers c
JOIN Orders o ON o.CustomerId == c.CustomerId
GROUP BY c.CustomerName
ORDER BY TotalOrders DESC;
```

#### Question 2: Design a simple database schema for an online library system. The system should track books, authors and borrowers. Each book can have multiple authors, and each borrower can borrow multiple books.

Authors:

| AuthorId | Name |
| -------------- | --------------- |
| 1 | Alice |
| 2 | Bob |
| 3 | Charlie |

Books:

| BookId | AuthorId | Name |
| --------------- | --------------- | --------------- |
| 1 | 1 | Book 1 |
| 1 | 2 | Book 1 |
| 2 | 2 | Book 2 |

Borrowers:

| BorrowerId | Name |
| --------------- | --------------- |
| 1 | Alice |
| 2 | Bob |

BorrowedBooks:

| BorrowerId | BookId |
| -------------- | --------------- |
| 1 | 1 |
| 1 | 2 |
| 2 | 3 |


### References
- [[Rocket Companies]]

