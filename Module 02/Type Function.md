# The `type()` function

## 1. What the `type()` function Does

The `type()` function in Python is used to determine the type of an object. 
* If you are unsure whether a given variable is integer, float, boolean, string or let's say a Data Structure (List, Tuple, etc.), you can use the type() function on the variable name
* A better knowledge of the 'type of the object' helps us apply appropriate operations on it
* It is useful to debug and understand the behavior of different variables and expressions

## 2. Code Examples

Here are a few examples to illustrate the use of the `type()` function:

<pre><code>
# Example 1: Finding the type of an integer
type(42)
# Output: &lt;class 'int'&gt;

# Example 2: Finding the type of a string
type("Hello, World!")
# Output: &lt;class 'str'&gt;

# Example 3: Finding the type of a list
type([1, 2, 3, 4, 5])
# Output: &lt;class 'list'&gt;

</code></pre>

Here the word `class` against the data type e.g. class 'int' indicates that the Integer object 42 belongs to the family of Integers

## 3. Variants of using `type()`

- **Using `type()` function output for comparison**: You can compare the `type()` function output against the data type to return `True` or `False`.

<pre><code>
number = 42
type(number) == int
# Output: True

type(number) == float
# Output: False
  
text = 'world'
type(text) == str
# Output: True

type(text) == bool
# Output: False

</code></pre>
