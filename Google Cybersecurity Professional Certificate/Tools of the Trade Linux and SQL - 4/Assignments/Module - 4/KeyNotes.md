# Key Notes - SQL and Databases

## Introduction to SQL and Databases

- A database is an organized collection of data stored electronically.
- A relational database stores data in related tables.
- SQL (Structured Query Language) is used to create, manage, and retrieve data from databases.
- Tables contain rows and columns:
  - Rows = records
  - Columns = fields/categories
- A primary key uniquely identifies each row in a table.
- A foreign key connects one table to another.
- Common data types:
  - String data → text/characters
  - Numeric data → numbers
  - Date and time data → timestamps, dates, login times
- SQL is commonly used in cybersecurity for:
  - Investigating logs
  - Tracking login attempts
  - Monitoring suspicious activity
  - Managing employee and device data

---

# SQL Queries

- `SELECT` retrieves data from a table.
- `FROM` specifies the table being queried.

Example:
```sql
SELECT firstname, lastname
FROM employees;
```

- `SELECT *` returns all columns.
- Queries usually end with a semicolon `;`.
- `ORDER BY` sorts query results.
- Default sorting is ascending.
- `DESC` sorts data in descending order.

Example:
```sql
SELECT customerid, city
FROM customers
ORDER BY city DESC;
```

- Multiple columns can be selected using commas.
- Multiple columns can also be used in sorting.

---

# More SQL Filters

- `WHERE` filters records based on conditions.

Example:
```sql
SELECT *
FROM employees
WHERE department = 'Marketing';
```

## Logical Operators

### AND
- Both conditions must be true.

```sql
WHERE department = 'Marketing'
AND office LIKE 'East%'
```

### OR
- Either condition can be true.

```sql
WHERE country = 'USA'
OR country = 'Canada'
```

### NOT
- Excludes matching records.

```sql
WHERE NOT country = 'USA'
```

## LIKE and Wildcards

- `LIKE` searches for patterns.
- `%` represents multiple unknown characters.
- `_` represents a single unknown character.

Example:
```sql
WHERE office LIKE 'East%'
```

## Comparison Operators

| Operator | Meaning |
|---|---|
| = | Equal to |
| != or <> | Not equal to |
| > | Greater than |
| < | Less than |
| >= | Greater than or equal to |
| <= | Less than or equal to |

## Aggregate Functions

### COUNT()
- Counts rows.

```sql
SELECT COUNT(firstname)
FROM customers;
```

### AVG()
- Returns average value.

### SUM()
- Returns total value.

---

# SQL Joins

- Joins combine data from multiple tables using related columns.

## INNER JOIN

- Returns only matching rows from both tables.

```sql
SELECT *
FROM employees
INNER JOIN machines
ON employees.device_id = machines.device_id;
```

## LEFT JOIN

- Returns all rows from the left table and matching rows from the right table.

```sql
SELECT *
FROM employees
LEFT JOIN machines
ON employees.device_id = machines.device_id;
```

## RIGHT JOIN

- Returns all rows from the right table and matching rows from the left table.

```sql
SELECT *
FROM employees
RIGHT JOIN machines
ON employees.device_id = machines.device_id;
```

## FULL OUTER JOIN

- Returns all rows from both tables.

```sql
SELECT *
FROM employees
FULL OUTER JOIN machines
ON employees.device_id = machines.device_id;
```

## Important Join Concepts

- `ON` specifies the matching column.
- Shared columns may need table names specified.
- Joins help combine related security data from different tables.
- Useful for:
  - Device tracking
  - Employee-machine mapping
  - Login investigations
  - Security monitoring

---

