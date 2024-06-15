# The `help()` Function

## 1. What the `help()` Function Does

The `help()` function is a built-in Python function that invokes the built-in help system. It is used to display the documentation of modules, functions, classes, keywords, etc. This is particularly helpful when you need to understand how to use a specific component in Python.

## 2. Code Examples

Here are a few examples to illustrate the use of the `help()` function:

<pre><code>
# Example 1: Getting help on the built-in `print` function
help(print)
# Output: (Displays the documentation for the print function)

# Example 2: Getting help on a specific module
import math
help(math)
# Output: (Displays the documentation for the math module)

# Example 3: Getting help on a specific class
help(str)
# Output: (Displays the documentation for the str class)
</code></pre>

## 3. Variants of Using `help()`

- **Interactive Help**: When used without arguments, `help()` enters an interactive help mode.

<pre><code>
help()
# Output: (Enters interactive help mode. Type "quit" to exit)
</code></pre>

Type "quit" to exit the help mode.

- **Help on Custom Functions**: You can use `help()` to get documentation on custom functions and classes if you include docstrings.

<pre><code>
def my_function():
    """This is a simple function that prints a message."""
    print("Hello from my_function!")

help(my_function)
# Output: Help on function my_function in module __main__:
#
# my_function()
#     This is a simple function that prints a message.
</code></pre>

