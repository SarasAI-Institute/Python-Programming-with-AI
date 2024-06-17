# Python Programming Basics

## 1) Syntax in Python

Python syntax refers to the rules that define how Python code should be written. It's like grammar rules in a language that ensure the computer understands what you want it to do.

Examples:
```python
# Example of an if statement
if 5 > 2:
    print("Five is greater than two!")

# Example of a for loop
for i in range(3):
    print(i)

# Example of defining a function
def greet(name):
    return f"Hello, {name}!"
print(greet("Alice"))

```

## 2) What is a Program in Python

A program in Python is a set of instructions written in Python code that tells the computer what tasks to perform. 
* It can range from simple scripts to complex applications.
* Programs are composed of functions, variables, and control structures that work together to achieve specific tasks, such as calculating values, processing data, or interacting with users.
```
# Example of a simple program
print("Hello, World!")

# Example of a program with variables and arithmetic operations
a = 10
b = 20
c = a + b
print(c)

# Example of a program with a function
def add(x, y):
    return x + y
print(add(5, 7))
```

## 3) Keywords in Python

Keywords are reserved words in Python that have special meanings and cannot be used as identifiers (such as variable names or function names). 
* They play a crucial role in defining the syntax and structure of Python programs.
* Examples include `if`, `else`, `for`, `while`, `def`, `class`, `import`, and `True`, `False`, `None` which are used for conditional statements, loops, defining functions, and more.

```
# Using the if keyword
if True:
    print("This is true")

# Using the for keyword
for i in range(3):
    print(i)

# Using the def keyword to define a function
def my_function():
    print("Hello from a function")
my_function()

```

## 4) Session or Workspace

A session or workspace refers to the environment where Python code is executed and where variables and data reside during program execution. 
* It includes memory space, imported modules, and the current state of variables.
* In interactive environments like Google Colab or Jupyter Notebooks, a session persists as long as the notebook is open, allowing for iterative code development and execution.
```
# Using variables in a session
x = 5
y = 3
print(x + y)  # Outputs: 8

# Variables persist in the session
z = x * y
print(z)  # Outputs: 15

# Session state with a function
def multiply(a, b):
    return a * b
result = multiply(4, 5)
print(result)  # Outputs: 20

```
## 5) Comments in Python

Comments in Python are text that are ignored when executing the program. 
* They are used to annotate code, provide explanations, and make it easier for others (or your future self) to understand the purpose and functionality of the code.
* Comments start with the `#` symbol and can be placed on a separate line or at the end of a line of code.

Example:
```python
# This is a comment explaining the next line of code
print("Hello, World!")  # This prints a greeting

# Comments can also be used to disable code
# print("This line won't run")

# Multiple comments for complex logic
# This function calculates the factorial of a number
def factorial(n):
    # If n is 0, return 1
    if n == 0:
        return 1
    else:
        # Otherwise, return n times the factorial of (n-1)
        return n * factorial(n-1)
print(factorial(5))  # Outputs: 120
```

## 6) Execution Flow of a Python Program
When you run a Python program, Python reads and executes your code line by line. It follows the instructions in the order they are written unless it comes across conditions or loops that change the flow.
```
# Sequential execution
print("First line")
print("Second line")

# Conditional execution
if 5 > 2:
    print("Five is greater than two!")
else:
    print("This should not print.")

# Loop execution
for i in range(3):
    print(f"Loop iteration {i}")

# Function calls
def greet(name):
    print(f"Hello, {name}!")
greet("Alice")
greet("Bob")

```

## 7) Integrated Development Environment (IDE) 
IDE is an application/platform/software that helps you write and run your Python programs more easily. It provides tools like a code editor, where you write your code, and features for running, testing, and debugging your programs. Below are the top five commonly used IDEs (Integrated Development Environments) for Python:
* Jupyter Notebook
* Visual Studio Code
* PyCharm
* SPYDER
* Atom


## 8) Commonly Used Keyboard Shortcuts in Google Colab
* Ctrl/Cmd + Enter: Run the current cell
* Shift + Enter: Run the current cell and move to the next cell
* Alt + Enter: Run the current cell and insert a new cell below
* Esc + A: Insert a code cell above
* Esc + B: Insert a code cell below
* Esc + M D: Delete the current cell
* Ctrl/Cmd + M M: Convert the current cell from code to text (markdown)
* Ctrl/Cmd + M Y: Change the current cell from text to code
* Ctrl/Cmd + M H: Show keyboard shortcuts
* Ctrl/Cmd + L : Comment or Uncomment code line(s)

