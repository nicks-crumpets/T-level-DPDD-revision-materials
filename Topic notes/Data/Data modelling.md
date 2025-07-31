# Data modelling

Data modelling can show how data is collected, stored and used by a business or organisation, make sure data is clear, accurate and consistent.

Also:

- How to use diagrams and graphs can help you find trends and patterns and their relationship to each other
- It can be shown at different levels depending on its purpose
- How to design databases, solve problems and make decisions

# Types of data modelling

Conceptual

Data model represents entities and their relationships at a high level not including keys, implementation etc. Used to communicate  a concept

Logical

Defines the structure pf data element and sets the relationships between them, attributes primary and foreign keys and normalisation 

Physical data model

Specific implementation of the data model, including table and column names, data types, indexes and other technical details, used to optimise a databases performance and integrity

**Hierarchical**

Organises data in a tree like structure where each parent note can have one or more child nodes, but each child node can have only one parent note, used for simple and fast retrieval of data

Relational

Organises data in tables where each row represents an entity instance and each column represents an attribute. Tables are linked by foreign keys that reference the primary keys of the other tables, used to manipulate data that follows set based logic efficiently

## Conceptual models examples

**Book**: Contains information about each book in the store, including its title, author, publisher, ISBN, publication date, and price.

**Category**: Represents a high-level category of books, such as "Fiction", "Non-Fiction",

**Sub-Category**: Represents a more specific category of books within a given Category, such as "Science Fiction", "Romance", "History", etc.

**Location**: Represents a physical location within the store where books are displayed and sold, such as "Front of Store", "Back of Store", "Children's Section", etc.

## Logical model examples

![image.png](Data%20modelling%201505301291278038ad95f5b4186707c2/image.png)

## Physical model example

![image.png](Data%20modelling%201505301291278038ad95f5b4186707c2/image%201.png)

## Relational model example

![image.png](Data%20modelling%201505301291278038ad95f5b4186707c2/image%202.png)

# Pros & Cons of hierarchical & relational models

| Aspect | Relational Models | Hierarchical Models |
| --- | --- | --- |
| Data structure | Structured using tables, rows & columns | Tree like structure with parent-child relationships |
| Flexibility | High flexibility due to relationships between tables | Limited flexibility, as data is organised in a strict hierarchy |
| Normalisation | Removed data redundancy and improves the data integrity | Data redundancy is common due to structure |
| Query language | SQL is widely supported | Custom query languages or proprietary methods |
| Scalability | Can handle large volumes of data and complex queries | Typically less scalable for complex queries and large datasets  |
| Ease of use | SQL is standardised and widely used | Requires specialised knowledge & tools for querying and managing data |
| Data Integrity | Strong data integrity through constraints and relationships | Data integrity can be compromised due to the structure |
| Use cases | Suitable for complex multi dimensional data with many relationships | Suitable for simple tree like data structures such as file systems  |

# What is data wrangling?

Cleaning, organising and improving raw data

It is designed to make the data easier to understand and use for analysis, like putting together a puzzle

It involves taking data from different sources and organising it into a useable format

The results of data wrangling results in people understanding the data better and making better decisions based on it

It is important after collecting data because raw data is inherently complex and difficult 

## Why?

Data needs to be understandable and analysable, without proper preparation, data related projects can fail and decision making may take far too long to be worthwhile, or data be bias or misinterpreted.

Data wrangling helps to convert raw data into useable/functional formats that can be easily analysed and used to make strategic decisions

Converting raw data into indexed & searchable datasets enables businesses to gather intelligence and make informed decisions

# Steps of data wrangling

## Step 1: Data discovery

Focussing on understanding the structure and content of the data, identifying and issues or challenges that may need to be addressed and define the questions, goals etc of the analysis

## Step 2: Data structuring

Involved structuring the data for analysis, including tasks such as transforming data formats, aggregating data and creating new columns or datasets

## Step 3: Data cleaning

Identifying and addressing any data quality issues or errors that may effect the accuracy or completeness of the analysis, such as handling missing or inconsistent data

## Step 4: Data Enriching

Additional data is added to the analysis to provide context or additional insights, such as joining external data sources

## Step 5: Data Validating

Accuracy and completeness of data are validated to ensure that the analysis is based on reliable and trustworthy data, such as running data quality checks

## Step 6: Data publishing

Analysis is presented to stakeholders, or published for broader consumption. Focusses on making the insights accessible and understandable to the intended audience, such as by creating visualisations