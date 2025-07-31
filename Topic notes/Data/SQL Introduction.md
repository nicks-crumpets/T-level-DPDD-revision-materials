# SQL Introduction

SQL - Structured Query Language

SQL is a standard programming language, most often used to manage and manipulate relational style databases. It allows creation, reading and deletion of data, abbreviated as CRUD.

It is widely used in various industries for data management and is essential for careers in data analysis, software development and most commonly database administration

# What’s in a database?

Firstly, a database itself is simply an organised collection of data

A relational database is the same, but it stores data in tables with rows & columns, the tables are connected through relationships

Examples of relational database programming languages are: MySQL, PostgreSQL,  and oracle database

**Tables** - Where data is stored in rows & columns

**Queries** - Commands to interact with the database

**Schemas** - Structure of the database, including tables & relationships

**Primary Keys** - Unique identifiers for table records

## So what’s a query?

A request for data or information ***from*** a database, using SQL statements to perform tasks

Common SQL statements are:

- SELECT - Retrieves data
- **INSERT -** Adds new data
- **UPDATE -** Modifies existing data
- **DELETE -**  Removes data

## What does an SQL query look like?

This code *(below)* will fetch all of the data from the *‘students’* table

```sql
SELECT * FROM students;
```

SELECT * - Retrieves all columns from a table

FROM students; - Specifies the *‘students’* table

# History pit stop :)

![image.png](SQL%20Introduction%2015053012912780ec8a2dd99a3eee4c98/image.png)

*Professionally ~~stolen~~ extracted from a presentation*

# Key features of SQL

**Data definition language** - Commands to define database structure: CREATE, ALTER, DROP

**Data control language** - Commands to control access: GRANT, REVOKE

**Data manipulation language** - Commands to manipulate data: SELECT, INSERT, UPDATE, DELETE 

**Transaction control language** - Commands to manage transactions: COMMIT, ROLLBACK

## Basic SQL Commands

SELECT, WHERE, AS, CONCAT

# Okay, so what is NoSQL?

NoSQL (it’s not ‘no SQL’, sorry, it) stands for Not Only SQL

It’s a category of database systems that do not use relational models, it’s designed for distributed data stores with large data storage needs, examples of which are: MongoDB, Cassandra, and Redis 

## So what’s the difference (SQL VS NoSQL)?

**Data model**

- SQL uses **structured** tables
- NoSQL uses unstructured data (JSON, UML etc)

**Schema**

- SQL databases have a fixed schema (defining tables and types)
- NoSQL databases have dynamic schemas

**Scalability**

- SQL databases are vertically scalable, to handle more, a server is upgraded
- NoSQL databases are horizontally scalable, designed to spread over multiple servers

## SQL commands explained

### SELECT

Retrieves records

For all: SELECT *

For certain: SELECT X FROM x;

### Renaming/AS

SELECT column AS “<new name>”

SELECT firstname AS “First Name”

### Concatenation/CONCAT

SELECT CONCAT(column1, ‘ ‘, column2)

FROM db;

SELECT CONCAT(firstname, ‘ ‘ , lastname)

FROM db;

## Types of functions

Aggregate - A function that takes all of the data and aggregates it into one value

Scalar - A function that applies to every row

## Aggregate

![image.png](SQL%20Introduction%2015053012912780ec8a2dd99a3eee4c98/image%201.png)

## Scalar

![image.png](SQL%20Introduction%2015053012912780ec8a2dd99a3eee4c98/image%202.png)

## WHERE

Commonly used for filtering 

WHERE countries = England

WHERE age = 44

WHERE Dylan = annoying (This could just use *)