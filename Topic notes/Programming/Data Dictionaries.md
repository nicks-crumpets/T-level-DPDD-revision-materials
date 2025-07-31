# Data Dictionaries

**“Dictionaries are a collection of unordered changeable keys/values”**

Part of a physical data model that has detail about each entry and its attributes

The data included in a data dictionary is:

- Table name - Name of the table (names must be unique among tables in the database)
- Field name - Each field is identified
- Field datatype - Datatype allocated to a field (INT, STR, BOOL etc)
- Field length - Allocated min/max length for a fields contents
- Field default value - This is stored if there is a default value for a field that should appear on the creation of a new record
- Field validation - Any validation in a field (Must be in format DD/MM/YYYY)
- Table security - Access permissions for a given user (read, write, delete, edit etc)
- Keys - Primary & foreign keys
- Indexes - Any indexed field
- Relationships - Any

# Operations

Add

Access an element x[name]

change an entry

```python
 x[’example’] = 28
```

# Add, change & delete

x[’example’] = 99

x[’example’] = 100

del x[’example’]

length of dictionary → len(x)

— List of dictionaries —

Add code, example of checking a users age against the age rating of a game

```python
users = [
	{"name" : "John", "id" : 1, "age":99},
	{"name" : "Steve", "id" : 2, "age":43},
	{"name" : "Ali", "id" : 3, "age":22},
```