The `SELECT` command in SQL is used to retrieve data from one or more tables in a database. Here’s a detailed explanation of its syntax and some examples:

### Basic Syntax

```sql
SELECT column1, column2, ...
FROM table_name
WHERE condition
GROUP BY column1, column2, ...
HAVING condition
ORDER BY column1, column2, ... ASC|DESC
LIMIT number;
```

### Explanation of Syntax

- **SELECT**: Specifies the columns that you want to retrieve. You can select specific columns or use `*` to select all columns.
- **FROM**: Specifies the table from which to retrieve the data.
- **WHERE**: Specifies the conditions for filtering the data.
- **GROUP BY**: Groups rows that have the same values in specified columns into aggregated data.
- **HAVING**: Specifies a condition for groups created by the `GROUP BY` clause.
- **ORDER BY**: Specifies the order of the result set. By default, it is in ascending order (`ASC`), but you can specify descending order (`DESC`).
- **LIMIT**: Specifies the number of records to return.

### Examples

1. **Select Specific Columns**

```sql
SELECT first_name, last_name
FROM employees;
```

This query retrieves the `first_name` and `last_name` columns from the `employees` table.

2. **Select All Columns**

```sql
SELECT *
FROM employees;
```

This query retrieves all columns from the `employees` table.

3. **Using WHERE Clause**

```sql
SELECT first_name, last_name
FROM employees
WHERE department = 'Sales';
```

This query retrieves the `first_name` and `last_name` of employees who work in the Sales department.

4. **Using GROUP BY and HAVING Clauses**

```sql
SELECT department, COUNT(*)
FROM employees
GROUP BY department
HAVING COUNT(*) > 5;
```

This query groups the employees by department and returns the departments with more than 5 employees.

5. **Using ORDER BY Clause**

```sql
SELECT first_name, last_name
FROM employees
ORDER BY last_name ASC;
```

This query retrieves the `first_name` and `last_name` of employees and sorts the result by `last_name` in ascending order.

6. **Using LIMIT Clause**

```sql
SELECT first_name, last_name
FROM employees
ORDER BY last_name ASC
LIMIT 10;
```

This query retrieves the `first_name` and `last_name` of employees, sorts the result by `last_name` in ascending order, and limits the result to the first 10 rows.

### Combining Multiple Clauses

```sql
SELECT first_name, last_name, department
FROM employees
WHERE department = 'Sales'
GROUP BY department
HAVING COUNT(*) > 2
ORDER BY last_name DESC
LIMIT 5;
```

This complex query:
- Selects `first_name`, `last_name`, and `department` columns.
- Filters rows where the `department` is 'Sales'.
- Groups the result by `department`.
- Filters groups with more than 2 employees.
- Orders the result by `last_name` in descending order.
- Limits the result to the first 5 rows.

These examples should give you a good understanding of how the `SELECT` statement works in SQL.