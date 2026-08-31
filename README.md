# Class Brief: Session 01 - Python Basics & Intro to Lists

**Date:** 18-06-2026
**Instructor:** Gaurav Singh  

---

## Overview
This session introduced the fundamentals of Python programming using Google Colab. We covered how to set up and navigate the coding environment, work with basic data types, utilize operators, manage variables, and touched upon our first data structure: Lists.

## What We Covered

* **Google Colab Environment:** 
  * Interface, navigation, and essential keyboard shortcuts.
  * Executing Python code cells and using Markdown for notes.
* **Python Data Types & Functions:** 
  * Understanding Integers, Floats, Strings (single, double, triple quotes), and Booleans.
  * Using `type()` to identify data types and structures.
  * Using `print()` to output strings and expression results.
* **Operators:** 
  * **Arithmetic:** `+`, `-`, `*`, and `/` (Note: `/` always returns a Float).
  * **Assignment:** Standard `=` and shorthand/augmented operators (`+=`, `-=`, `*=`, `/=`).
  * **Comparison:** `<`, `>`, `<=`, `>=`, `==` (equal to), `!=` (not equal to).
* **Variables in Depth:** 
  * Why we need them: storing data, reusing values, avoiding hard-coded data, and making dynamic programs.
  * How assignments work in complex mathematical operations.
  * Variable overwriting and their general limitations.
* **Introduction to Lists:** 
  * Why data structures are necessary (storing multiple values efficiently without needing dozens of variables).
  * Defining lists for mixed data (e.g., movie info) and numeric lists.
  * Applying built-in functions to numeric lists: `sum()`, `len()`, `max()`, and `min()`.

## Extra Tips & Best Practices
* **Colab Speed:** Memorize `Shift + Enter` to run your current cell and immediately move to the next one. It makes coding much faster!
* **Naming Variables:** Use `snake_case` for your variable names in Python (e.g., `user_age` or `final_score`). Also, never name a variable after a built-in Python function (like naming a variable `print` or `list`), as it will break that function's ability to work!
* **The Division Quirk:** Remember that the standard division operator `/` will *always* give you a float (e.g., `10 / 2` results in `5.0`). If you ever need it to round down to a whole integer, you'll want to use floor division `//`.
* **Testing Comparisons:** When using `==`, a common beginner mistake is accidentally using a single `=`. Remember: single `=` is for *assigning* a value, double `==` is for *asking a question* (Are these equal?).

---
*Got questions? Feel free to reach out during the next Q&A session!*

# Class Brief: Session 02 - Built-in Functions & Data Structures

**Date:** August 17, 2026  
**Instructor:** Gaurav Singh | Saras AI Institute  

---

## Overview
In this session, we leveled up our Python skills by exploring built-in functions and transitioning from single variables to organized collections of data. We learned how to interact with users, inspect Python objects, and build our very first data structures using Lists to handle heterogeneous (mixed) data.

---

## What We Covered & Concept Review

### 1. Python's Built-in Functions
Python comes with a toolbox of pre-written functions ready for us to use. These functions help us display information, get user input, and figure out how other parts of Python work.

*   **`print()`**: Displays output to the screen. (We no longer have to rely on putting variables at the bottom of the Colab cell!)
*   **`input()`**: Pauses the program and waits for the user to type something in.
*   **`type()`**: Tells us the data type of a value or variable.
*   **`help()`**: Pulls up the built-in documentation for a specific function or object.
*   **`dir()`**: Shows a list of all the attributes and methods available for an object.

```python
# Displaying a message
print("Welcome to Session 02!")

# Getting input from a user
user_name = input("What is your name? ")
print("Hello", user_name)

# Using help() to understand how print works
help(print)
```

### 2. The Need for Data Structures
Up until now, we used single variables (e.g., `score1 = 90`, `score2 = 85`). But what if we have 1,000 students? 
*   **The Problem:** Creating a new variable for every single piece of data is impossible to manage.
*   **The Solution:** Data Structures. They allow us to organize, manage, and store massive collections of data under a single name, making our code clean and efficient.
*   Python has several built-in data structures (Lists, Tuples, Dictionaries, Sets), but we started our focus on **Lists**.

### 3. Deep Dive: Lists & Heterogeneous Data
A list is exactly what it sounds like—an ordered sequence of items. One of the superpower features of Python lists is that they can be **heterogeneous**, meaning they can store different data types at the same time.

```python
# Creating a list of just strings (homogeneous)
tech_stack = ["Python", "React", "Node.js"]

# Creating a list with mixed data types (heterogeneous)
# Includes a String, Integer, Float, and Boolean
student_profile = ["Aman", 22, 85.5, True]

# Printing the entire list
print(student_profile)

# Checking the type of our data structure
print(type(student_profile))
# Output: <class 'list'>
```

---

## Extra Tips & Best Practices

*   **The `input()` Trap:** Whenever you use `input()`, Python **always** captures the user's answer as a String (`str`). If you ask a user for their age and want to do math with it, you must convert it to an integer first using `int()` (e.g., `age = int(input("Enter age: "))`).
*   **Stuck? Use `dir()` and `help()`:** You don't need to memorize everything! If you forget what you can do with a list, type `dir(list)` in Colab to see your options. Then, use `help()` to learn how to use a specific feature.
*   **List Readability:** Just because a list *can* hold mixed data types doesn't always mean it *should*. Grouping related data makes your code easier to read. Use logical variable names (e.g., `student_grades` for numbers, `student_details` for mixed profile info).

---

## Additional Resources
*   [Python Built-in Functions (Official Docs)](https://docs.python.org/3/library/functions.html) - *The complete list of Python's built-in tools.*
*   [Python Lists Explained (W3Schools)](https://www.w3schools.com/python/python_lists.asp) - *A great visual guide to creating and using lists.*

---

*Got questions? Open an issue in this repository, post in the discussion forums, or bring them to our next live support session!*