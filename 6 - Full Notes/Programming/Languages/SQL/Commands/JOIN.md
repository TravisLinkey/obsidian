
2024-09-02 19:58

Tags: [[SQL]]

### Overview
`JOIN` is used to combine rows from two or more tables based on a related column between them.

#### Example
```sql
SELECT employees.name, departments.department_name
FROM employees
INNER JOIN departments ON employees.department_id = departments.department_id;
```
This query retrieves the names of employees and the corresponding department names by matching the `department_id` from `employees` table with the `department_id` in the `departments` table.

### References
- [[Interview Prep]]
- [[Left Join]]
- [[Right Join]]
- [[Inner Join]]
