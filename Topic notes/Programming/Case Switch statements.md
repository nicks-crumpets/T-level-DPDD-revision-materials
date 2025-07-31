# Case/Switch statements

Used instead of if/elif(else-if) statements when code contains multiple choices.

It’s a selection control mechanism (A way to select an option)

It allows the value of a variable or expression to change the flow of program execution

```python
choice = input("Make a selection between 1 and 5: ")

match choice:
	case "1":
		print("You selected 1")
	case "2":
		print("You selected 2")
	case "3":
		print("You selected 3")
	case "4":
		print("You selected 4")
	case "5":
		print("You selected 5")
		
	case _:
		print("You didn't select a valid option")

```

So if you typed one of the available inputs, your input is matched to one of the available cases, and the code under the case is run

If you try to enter a value that is not listed the possible ‘cases’, then ‘case _’ will run, as it catches any input that hasn’t been matched