# SQL Operators

*When typing SQL queries make sure to end them with ‘;’*

## Comparison operators

```sql
10 > 20 --false
10 < 20 --true
10 <= 20 --true
10 >= 9 --true
0 = 0 --true
1 != 0 --true
```

## Equal to

Checks if the given values are equal, if they are, returns ‘true’

```sql
0 = 0 --true
'Paul' = 'paul' --false
```

## Not equal to

Checks if the values are *not* equal, if its *not equal* it returns ‘true’

```sql
0 != 0 --false
0 <> 1 -- true
```

## Greater than & Less than

Checks if the value is larger than another set/given value, if greater or less than respectively, returns ‘true’

```sql
--Greater than 
10 > 0 --true
0 > 10 --false
'abc' > 'ace' --true
--Less than
0 < 1 -- true
```

## Greater than or equal to & Less than or equal to

Checks if the value is larger or less than equal to the other given/set value, if it is respective then it returns true

```sql
--Greater than or equal to
2 >= 1 --true
2 >= 2 -- true
--Less than or euqal to
0 <= 1 --true
2 <= 2 --true
```

## Operator Precedence

Certain operators have priority over others

It’s the same style as BODMAS/BIDMAS

*Brackets, Indices (powers), Division, Multiplication, Addition and Subtraction*

### Equal priorities

If the operators have equal priorities then the operators are treated directionally from left to right or right to left

Brackets, multiplication & division, AND, & or → Left to Right

Subtraction & addition, and NOT → Right to left

![image.png](SQL%20Operators%2015453012912780f4ab8ffd9ef9b184bd/image.png)

```sql
SELECT town, age
FROM customers
WHERE age = 24 AND town = 'Reading' OR town = 'Redruth';
```

```sql
SELECT town, age
FROM customers
WHERE age = 24 AND town = 'Reading' 
OR  age = 24 AND town = 'Redruth';
```

Or, this could be written in a simpler way

```sql
SELECT town,gender FROM customers
WHERE age = 24 AND (town = 'Reading' OR town = 'Redruth);
```

And it can get more complicated…

Filter 1

- Salary > 10,000
- From Redruth
- Gender: Female

Filter 2

- Between 21 and 29
- Salary lower than or equal to 20,000
- Female

```sql
(
		Salary > 1000 AND town = 'Redruth'
			OR(
				(age > 20 AND age < 30)
				AND salary <= 20000
			)
)
AND gender = 'F';
```