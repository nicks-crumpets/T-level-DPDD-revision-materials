# Filtering Data with SQL

# General data filtering

```sql
SELECT Name
FROM users
WHERE Role = "Manager";
```

Filtering data is the base level of any query, particularly when you want to filter multiple conditions

## **Filtering *two* columns - AND Keyword**

```sql
SELECT firstName, lastName
FROM users
WHERE firstName = 'Kiera' AND lastName = 'Glover' AND firstName = 'Jennifer';
```

## **OR keyword**

```sql
SELECT firstName, lastName
FROM users
WHERE firstName = 'Kiera' AND lastName = 'Glover' OR firstName = 'Jennifer';
```

## **The NOT Keyword**

```sql
SELECT firstName, lastName
FROM users
WHERE NOT firstName = 'Jen';
```