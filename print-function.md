# The `print()` Function

## 1. What the `print()` Function Does

The `print()` function is one of the most commonly used functions in Python. 
* It outputs text to the console or terminal.
* It is crucial for displaying results, debugging, and providing user feedback.

## 2. Simple Application

Here are a few basic examples to illustrate the use of the `print()` function:

<pre><code>
# Example 1: Printing a simple message
print("Hello, World!")
# Output: Hello, World!

# Example 2: Printing numbers
print(42)
# Output: 42

# Example 3: Printing multiple items
print("The answer is", 42)
# Output: The answer is 42
</code></pre>

## 3. Application to understand code behaviour and output

<pre><code>
# Example 1: Observing what values does range(5) contain
  for i in range(5):
    print(i)

# Example 2: Understanding how the code generates intermediate outputs
  nums = []
  for i in range(5):
    nums.append(i)
    print(nums)
</code></pre>

## 4. Variants of Using `print()`

The `print()` function has several optional parameters that allow you to customize its behavior.

- **Multiple Arguments**: You can print multiple items by separating them with commas.

<pre><code>
print("Python", "is", "fun")
# Output: Python is fun
</code></pre>

- **Custom Separator**: By default, `print()` separates items with a space. You can change this using the `sep` parameter.

<pre><code>
print("Python", "is", "fun", sep="-")
# Output: Python-is-fun
</code></pre>

- **Custom End Character**: By default, `print()` ends with a newline character. You can change this using the `end` parameter.

<pre><code>
print("Hello, World!", end=" :) ")
print("Python is amazing!")
# Output: Hello, World! :) Python is amazing!
</code></pre>

- **File Output**: You can direct the output to a file using the `file` parameter.

<pre><code>
with open('output.txt', 'w') as f:
    print("This will be written to the file.", file=f)
# Output: (Written in output.txt) This will be written to the file.
</code></pre>
