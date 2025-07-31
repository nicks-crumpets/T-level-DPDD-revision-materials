# BETWEEN, LIKE, AT

*Queries continued*

# BETWEEN

```sql
SELECT <coloumn>
FROM <table>
WHERE <column> BETWEEN X AND Y
```

# IN

```sql
SELECT * FROM <table>
WHERE <column> IN (value1, value2...)
```

Or, the looooong way…

```sql
SELECT * FROM employees
WHERE emp_no = 10001 or emp_no = 2009....

```

# Partial lookups

## LIKE

```sql
SELECT first_name FROM employees
WHERE first_name LIKE 'P%':
```

% → any number of characters

_ → One character

**Add in the wildcards table from the presentation**

## Type casting

```sql
SELECT * FROM your_table
WHERE CAST(your_numeric_column AS VARCHAR) LIKE '2%'
```

This won’t change the database, as it is just type casting for the query

/hea