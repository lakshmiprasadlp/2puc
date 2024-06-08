# C++ Operators

## Table of Contents
1. [Arithmetic Operators](#arithmetic-operators)
2. [Assignment Operators](#assignment-operators)
3. [Comparison Operators](#comparison-operators)
4. [Logical Operators](#logical-operators)
5. [Bitwise Operators](#bitwise-operators)

## Arithmetic Operators
Arithmetic operators are used to perform common mathematical operations.

| Operator | Description | Example |
|----------|-------------|---------|
| +        | Addition    | `a + b` |
| -        | Subtraction | `a - b` |
| *        | Multiplication | `a * b` |
| /        | Division    | `a / b` |
| %        | Modulus     | `a % b` |
| ++       | Increment   | `++a` or `a++` |
| --       | Decrement   | `--a` or `a--` |

## Assignment Operators
Assignment operators are used to assign values to variables.

| Operator | Description | Example |
|----------|-------------|---------|
| =        | Assign      | `a = b` |
| +=       | Add and assign | `a += b` (equivalent to `a = a + b`) |
| -=       | Subtract and assign | `a -= b` (equivalent to `a = a - b`) |
| *=       | Multiply and assign | `a *= b` (equivalent to `a = a * b`) |
| /=       | Divide and assign | `a /= b` (equivalent to `a = a / b`) |
| %=       | Modulus and assign | `a %= b` (equivalent to `a = a % b`) |

## Comparison Operators
Comparison operators are used to compare two values. They return a boolean value (`true` or `false`).

| Operator | Description | Example |
|----------|-------------|---------|
| ==       | Equal to    | `a == b` |
| !=       | Not equal to| `a != b` |
| >        | Greater than| `a > b` |
| <        | Less than   | `a < b` |
| >=       | Greater than or equal to | `a >= b` |
| <=       | Less than or equal to | `a <= b` |

## Logical Operators
Logical operators are used to perform logical operations.

| Operator | Description | Example |
|----------|-------------|---------|
| &&       | Logical AND | `a && b` |
| \|\|     | Logical OR  | `a \|\| b` |
| !        | Logical NOT | `!a` |

## Bitwise Operators
Bitwise operators are used to perform bit-level operations.

| Operator | Description | Example |
|----------|-------------|---------|
| &        | AND         | `a & b` |
| \|       | OR          | `a \| b` |
| ^        | XOR         | `a ^ b` |
| ~        | NOT         | `~a` |
| <<       | Left shift  | `a << b` |
| >>       | Right shift | `a >> b` |

### Bitwise Operators Explained
- **& (AND)**: Performs a bitwise AND operation.
- **\| (OR)**: Performs a bitwise OR operation.
- **^ (XOR)**: Performs a bitwise XOR operation.
- **~ (NOT)**: Inverts all the bits.
- **<< (Left Shift)**: Shifts bits to the left by a specified number of positions.
- **>> (Right Shift)**: Shifts bits to the right by a specified number of positions.

## Examples

### Arithmetic Operator Example
```cpp
#include <iostream>

int main() {
    int a = 10, b = 5;
    std::cout << "a + b = " << (a + b) << std::endl;
    std::cout << "a - b = " << (a - b) << std::endl;
    std::cout << "a * b = " << (a * b) << std::endl;
    std::cout << "a / b = " << (a / b) << std::endl;
    std::cout << "a % b = " << (a % b) << std::endl;
    return 0;
}
