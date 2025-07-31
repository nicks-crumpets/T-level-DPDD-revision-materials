# DISTINCT, GROUP BY, ORDER BY & LIMIT

# DISTINCT

Returns unique values from a selected column or set of columns

Helps to eliminate any duplicate results

```sql
SELECT DISTINCT <coloumn1>, <coloumn2>
FROM <table>
```

Returns the unique values from the specified columns removing duplicate rows

Input the table from the presentation for DISTINCT syntax

Used for inventory management

## Grouping data (GROUP BY)

```sql
SELECT COUNT("Type1") AS "Pokemon Count"
FROM pokemon;
```

Finding how many types of Pokemon there are

Add the table on the right of the pres.

```sql
SELECT COUNT("Type1) AS "Pokemon Count"
FROM Pokemon
GROUP BY "Type 1";
```

Successfully finds how many types of Pokemon there are

This data will look rather messy, because there’s no order!…

## GROUP BY

```sql
SELECT COUNT("Type1") AS "Pokemon Count"
FROM pokemon
GROUP BY "Type 1"
ORDER BY "Pokemond Count"DESC;
```

DESC is descending order

ASC is ascending order

## LIMIT

```sql
SELECT * FROM dc
LIMIT 5;
```

Allows you to *limit* what is seen in the information