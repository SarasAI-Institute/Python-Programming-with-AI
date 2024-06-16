
## **Arithmetic Operators**
* Arithmetic are fundamental in numerical computations
* They are used extensively in mathematical calculations, ranging from basic arithmetic in everyday calculations to complex formulas in scientific and engineering applications

| Symbol | Description                    | Code Example     | Code Output |
|--------|:--------------------------------|------------------|-------------|
| +      | Addition                       | `print(10 + 2)`  | `12`        |
| -      | Subtraction                    | `print(8 - 4)`   | `4`         |
| *      | Multiplication                 | `print(7 * 5)`   | `35`        |
| /      | Division                       | `print(10 / 2)`  | `5.0`       |
| %      | Modulus (returns remainder)    | `print(9 % 4)`   | `1`         |
| //     | Floor Division (returns quotient) | `print(27 // 5)` | `5`       |
| **     | Exponentiation                 | `print(2 ** 3)`  | `8`         |

---
## **Comparison Operators**
* Comparison operators are fundamental for decision-making processes in programming
* They are used to compare values and expressions, returning boolean results (`True` or `False`)
* They are essential in conditional statements (`if`, `else`, `elif`) and looping constructs (`while`, `for`) to control the flow of a program based on conditions

| Symbol | Description           | Code Example     | Code Output |
|--------|:-----------------------|------------------|-------------|
| >      | Greater than          | `print(10 > 2)`  | `True`      |
| <      | Less than             | `print(8 < 4)`   | `False`     |
| >=     | Greater than equal to | `print(7 >= 5)`  | `True`      |
| <=     | Less than equal to    | `print(10 <= 2)` | `False`     |
| ==     | Equal to              | `print(9 == 4)`  | `False`     |
| !=     | Not Equal to          | `print(27 != 5)` | `True`      |

---

## **Assignment Operators**
* Assignment operators are crucial for storing and manipulating data throughout the execution of a program
* They are used to assign values to variables and modify their contents
* They provide a shorthand way of updating variables based on their current values, improving code efficiency and readability

  
| Symbol | Description | Code Example | Code Output |
|--------|:-------------|--------------|-------------|
| =      | Assigns the value or result of the expression on the right to the variable on the left. | `x = 5`<br>`print(x)` | `5` |
| +=     | Overwrites the earlier value of x by adding the specified value.<br> Note : `x += 10` is the same as `x = x + 10`. | `x = 5`<br>`x += 10`<br>`print(x)` | `15` |
| -=     | Overwrites the earlier value of x by subtracting the specified value.<br> Note : `x -= 10` is the same as `x = x - 10`. | `x = 20`<br>`x -= 6`<br>`print(x)` | `14` |
| \*=    | Overwrites the earlier value of x by multiplying the specified value.<br> Note : `x *= 10` is the same as `x = x * 10`. | `x = 7`<br>`x *= 2`<br>`print(x)` | `14` |
| /=     | Overwrites the earlier value of x by dividing the specified value.<br> Note : `x /= 10` is the same as `x = x / 10`. | `x = 50`<br>`x /= 10`<br>`print(x)` | `5.0` |

---

## **Logical Operators**
* Logical operators are commonly used in decision-making and control flow statements to determine the outcome based on multiple conditions
* They are used to combine or manipulate boolean values (`True` or `False`)
* They are essential in boolean algebra and conditional logic, allowing complex conditions to be expressed concisely

| Operator | Description                               | Example               | Result   |
|----------|-------------------------------------------|-----------------------|----------|
| `and`    | Returns True if both statements are true.  | `True and False`      | `False`  |
| `or`     | Returns True if one of the statements is true. | `True or False`   | `True`   |
| `not`    | Reverse the result, returns False if the result is true. | `not True`  | `False`  |

---

## **Membership Operators**
* Membership operators are used to test for membership in a sequence (such as lists, tuples, strings, or dictionaries).
* They are essential for checking the presence or absence of a value within a data structure, facilitating data validation, searching, and filtering operations

| Operator | Description                               | Example               | Result   |
|----------|-------------------------------------------|-----------------------|----------|
| `in`     | Returns True if the specified value is found in the given sequence. | `5 in [1, 2, 3]`   | `False`  |
| `not in` | Returns True if the specified value is not found in the given sequence. | `5 not in [1, 2, 3]` | `True` |

---

## **Bitwise Operators**
* Bitwise operators are used in low-level programming, hardware manipulation, cryptography, and optimization algorithms where efficiency is critical
* They are used to manipulate individual bits of integers at a binary level
* They offer powerful tools for working directly with binary data and performing bit-level operations

| Operator | Description                               | Example               | Result   | Explanation                                               |
|----------|-------------------------------------------|-----------------------|----------|-----------------------------------------------------------|
| `&`      | Bitwise AND                                | `5 & 3`               | `1`      | 5 in binary is `101`, 3 in binary is `011`. Bitwise AND gives `001` which is 1 in decimal. |
| `\|`     | Bitwise OR                                 | `5 \| 3`              | `7`      | 5 in binary is `101`, 3 in binary is `011`. Bitwise OR gives `111` which is 7 in decimal. |
| `^`      | Bitwise XOR                                | `5 ^ 3`               | `6`      | 5 in binary is `101`, 3 in binary is `011`. Bitwise XOR gives `110` which is 6 in decimal. |
| `~`      | Bitwise NOT                                | `~5`                  | `-6`     | Bitwise NOT inverts the bits of the number and gives the two's complement of the number minus one. For example, `~5` inverts `101` to `010`, which is `-6` in two's complement form. |
| `<<`     | Left shift                                 | `5 << 1`              | `10`     | Left shift moves the bits to the left by the specified number of positions. 5 in binary `101` becomes `1010` which is 10 in decimal. |
| `>>`     | Right shift                                | `5 >> 1`              | `2`      | Right shift moves the bits to the right by the specified number of positions. 5 in binary `101` becomes `10` which is 2 in decimal. |


