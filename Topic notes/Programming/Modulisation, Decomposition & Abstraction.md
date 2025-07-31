# Modularisation, Decomposition & Abstraction

# Modularisation

**“The process of dividing a program into separate sub-programs”**

Commonly used in OOP (Object oriented programming), and when making code libraries (simple ones are just a single module)

Modules are separate software components and can be used in various apps & functions in the program

# Decomposition

**“Breaking down a complicated program into smaller tasks”**

## Four steps of decomposition

1. Identify and describe the problems and processes
2. Break down the problems into separate tasks - Beginning to decompose the problem, top down method is often used when the problem is known
3. Describe the tasks and subtasks - Requiring documentation to be created that is clear and allows a third party to implement the solution to the problem
4. Communicate - Once decomposed the team making the program should all be given an overview as well as assigned modules to work on

# Abstraction

The process of removing details and/or characteristics that aren’t needed, to focus on what is essential

## The London underground map

A well known example, as the real world distances aren’t included, as they’re irrelevant to planning a journey, taking the map from extremely hard to understand, to a simple map

![image.png](Modulisation,%20Decomposition%20&%20Abstraction%202544d8936d0a4b76938659184f392b57/image.png)

Abstraction helps to solve problems by removing detail that doesn’t help to solve the problem, preventing it from getting in the way later

A generalised idea of a program after it is abstracted is known as a ‘model’

## The main steps of abstraction

1. Information needed to solve a problem should be identified, otherwise the solution might not actually solve the problem. Also it’s important to know **why** the information is needed (& information format too)
2. Carry out abstraction to filter any unnecessary information

Each layer of abstraction should show:

- Inputs - What is inputted to the system at a given level (Currency @ 2dp)
- Outputs - How and in what format the output is displayed (Graph, tabular data etc)
- Variables - Any that are used in a given layer
- Constants  - Any that are used in a given layer
- Key processes - Anything that the layer needs to **do**
- Repeated processes - Anything done multiple times in the system