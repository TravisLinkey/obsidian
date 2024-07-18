
2024-07-17 14:51

Tags: [[Relational Database]] | [[SQL]]

A type of join in [[SQL]] that returns all rows from the left table and the matching rows from the right table.

If there is not match, the result is NULL on the right side of the table.

```sql
SELECT columns
FROM left_table
LEFT JOIN right_table
ON left_table.common_column = right_table.common_column;

```
### Example

#### Employees
| EmployeeID | Name | DepartmentId |
| --------------- | --------------- | --------------- |
| 1 | John Doe | 1 |
| 2 | Jane Smith | 2 |
| 3 | Sam Brown | 3 |
| 4 | Lisa Black | NULL |

#### Departments
| DepartmentId | DepartmentName |
| -------------- | --------------- |
| 1 | HR |
| 2 | Finance |

```sql
SELECT Employees.EmployeeID, Employees.Name, Departments.DepartmentName
FROM Employees
LEFT JOIN Departments ON Employees.DepartmentID = Departments.DepartmentID;

```

#### Results
| EmployeeId | Name | DepartmentName |
| --------------- | --------------- | --------------- |
| 1 | John Doe | 1 |
| 2 | Jane Smith | 2 |
| 3 | Sam Brown | NULL |
| 4 | Lisa Black | NULL |

### Explanation
In this result, all employees are listed, but only those who have a matching `DepartmentId` in the `Departments` table have their `DepartmentName` shown. For employees without a matching `DepartmentId`, the `DepartmentName` is **NULL**


### References
- [[SQL]]

