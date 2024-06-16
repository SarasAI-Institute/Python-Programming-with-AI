
## **Arithmetic Operators**

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

| Symbol | Description | Code Example | Code Output |
|--------|:-------------|--------------|-------------|
| =      | Assigns the value or result of the expression on the right to the variable on the left. | `x = 5`<br>`print(x)` | `5` |
| +=     | Overwrites the earlier value of x by adding the specified value.<br> Note : `x += 10` is the same as `x = x + 10`. | `x = 5`<br>`x += 10`<br>`print(x)` | `15` |
| -=     | Overwrites the earlier value of x by subtracting the specified value.<br> Note : `x -= 10` is the same as `x = x - 10`. | `x = 20`<br>`x -= 6`<br>`print(x)` | `14` |
| \*=    | Overwrites the earlier value of x by multiplying the specified value.<br> Note : `x *= 10` is the same as `x = x * 10`. | `x = 7`<br>`x *= 2`<br>`print(x)` | `14` |
| /=     | Overwrites the earlier value of x by dividing the specified value.<br> Note : `x /= 10` is the same as `x = x / 10`. | `x = 50`<br>`x /= 10`<br>`print(x)` | `5.0` |

---

## **Logical Operators**

| Operator | Description                               | Example               | Result   |
|----------|-------------------------------------------|-----------------------|----------|
| `and`    | Returns True if both statements are true.  | `True and False`      | `False`  |
| `or`     | Returns True if one of the statements is true. | `True or False`   | `True`   |
| `not`    | Reverse the result, returns False if the result is true. | `not True`  | `False`  |

---

## **Membership Operators**

| Operator | Description                               | Example               | Result   |
|----------|-------------------------------------------|-----------------------|----------|
| `in`     | Returns True if the specified value is found in the given sequence. | `5 in [1, 2, 3]`   | `False`  |
| `not in` | Returns True if the specified value is not found in the given sequence. | `5 not in [1, 2, 3]` | `True` |

---

## **Bitwise Operators**

| Operator | Description                               | Example               | Result   | Explanation                                               |
|----------|-------------------------------------------|-----------------------|----------|-----------------------------------------------------------|
| `&`      | Bitwise AND                                | `5 & 3`               | `1`      | `5` in binary is `101`, `3` in binary is `011`. Bitwise AND gives `001` which is `1` in decimal. |
| `\|`     | Bitwise OR                                 | `5 \| 3`              | `7`      | `5` in binary is `101`, `3` in binary is `011`. Bitwise OR gives `111` which is `7` in decimal. |
| `^`      | Bitwise XOR                                | `5 ^ 3`               | `6`      | `5` in binary is `101`, `3` in binary is `011`. Bitwise XOR gives `110` which is `6` in decimal. |
| `~`      | Bitwise NOT                                | `~5`                  | `-6`     | Bitwise NOT inverts the bits of the number and gives the two's complement of the number minus one. For example, `~5` inverts `101` to `010`, which is `-6` in two's complement form. |
| `<<`     | Left shift                                 | `5 << 1`              | `10`     | Left shift moves the bits to the left by the specified number of positions. `5` in binary `101` becomes `1010` which is `10` in decimal. |
| `>>`     | Right shift                                | `5 >> 1`              | `2`      | Right shift moves the bits to the right by the specified number of positions. `5` in binary `101` becomes `10` which is `2` in decimal. |


