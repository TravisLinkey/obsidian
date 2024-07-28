
2024-07-27 07:50

Tags: [[SQL]] | [[Practice]]

### Question: Show patient_id and first_name from patients where their first_name start and ends with 's' and is at least 6 characters long.

```sql
SELECT patient_id, first_name
FROM patients
WHERE first_name LIKE "s____%s";
```

### Question: Display every patient's first_name. Order the list by the length of each name and then by alphabetically.

```sql
SELECT first_name
FROM patients
ORDER BY LEN(first_name), first_name
```

