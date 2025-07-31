# Creating tables

```sql
CREATE TABLE table_name (
column1 datatype,
column2 datatype,
...
);
```

Data types in SQL

Numeric - INT, Decimal, float

Character types - Char, var char, text

Date & time - Dates, times, timestamps

# Primary keys & constraints

## Primary key

Uniquely identifies each record in a table

constraints

Not Null, column cannot be null

Unique, ensures all values are unique

Check, Validates data based on a condition

# Create table syntax

## Insert into syntax

```sql
INSERT TABLE table_name(column1 2,...)
Values(1, 2, 3....)
```

```sql
INSERT INTO Employees (ID, Name, Salary)
VALUES(1,'Peter Parker',60000);
```

```sql
INSERT INTO(ID, Name, Salary)
VALUES
(2,'Hawkeye',66000);
(2,'Bruce Banner',70000);
```

## Foreign keys and table relationships

A foreign key is a field in one table that uniquely identifies a row of another table

```sql
CREATE TABLE Orders(
ORDERID INT PRIMARY KEY
|
|
\/
```

## Inserting data with relationships

Insert data into then parent table (customers)

Insert data into the child database (orders), referencing the parent table

```sql
-- Insert into customers 
INSERT INTO Customers(CustomerID, Name)
VALUES(1, 'Tony Stark');

-- Insert into orders
INSERT INTO Orders(OrderID, OrderDate, CustomerID)
Values(101,'2023-10-01',1);
```

customer

orders

products