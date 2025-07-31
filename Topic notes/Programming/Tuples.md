# Tuples

A collection which is ordered and unchangeable

Tuples are written with round brackets

Once a tuple is created you can’t change its values, they’re unchangeable and immutable

```python
thistuple = ('apple', 'banana', 'cherry')
print(thistuple)
```

To change them they must be converted to a list

 

```python
thistuple = ('apple', 'banana', 'cherry')
thistuple[3] = "orange" # this will cause an error, 3 doesn't exist
print(thistuple)
```

# Tuples with one item (special case)

```python
thistuple = ("apple",) # Must have the comma even with one 
```

Tuples should be used when the variable doesn’t *ever* need to be changed

## Python sets

```python
a = {1, 2, 3, 4, 5}
b = {4, 5, 6, 7, 8,}

print( "Union", a|b )
print( "Union", a.union(b))

print( "Intersection", a&b.....
```