
2024-09-02 19:58

Tags: [[SQL]]

### Overview
`GROUP BY` is used to arrange identical data into groups.

It is commonly used with aggregate functions, (`COUNT`, `SUM`, `AVG`) to summarize information.

#### Example
```sql
SELECT department, COUNT(employee_id)
FROM employees
GROUP BY department;
```
This groups employees by department and then counts the number of employees in each department.

### References
- [[Interview Prep]]
