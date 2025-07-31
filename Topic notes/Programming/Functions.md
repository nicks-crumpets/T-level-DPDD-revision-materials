# Functions

*“A function is code which is written to perform a specified task and  can be used many times in a program”*

# The 3 types of functions (In Python)

## Built in functions

Functions that are built into python (as the name suggests). E.g:

```python
# Built in length function
my_list_length = len(my_list)
```

## User defined functions

Functions created by the developer

```python
def sausages():
	print("Sausages are the best!")
	life = 42
	print("The meaning of life is: ", life)
```

## Anonymous/Lambda functions

Functions that are not declared using the ‘def’ keyword

# Methods vs Functions

Simply, a method is a function which is **also** part of a class and accessed using an instance or an object of the class it’s part of.

A function however, is not restricted, it’s standalone

*All methods are functions, but not all functions are methods*

# Function code

## Creating a function

```python
def my_perfect_function():
	print("The best function that anyone's ever seen, ever")
```

## Calling a function

```python
my_amazing_function()
```

# Anonymous functions

The study guide never mentions the need to know how they work, but it can come in useful

```python
lambda parameter(s) : expression
```

So a practical example looks like this:

```python
adding = lambda a,b : a + b

print(adding(2,3))
```

bUt WhAt’S tHe PoInT oF tHeM?!!?

Lambda is another way of writing a small expression as a function that’s not named

Also, you can define a lambda function and pass it to a function in a single step, rather than having to go through a function name

So long story short, because it’s quicker