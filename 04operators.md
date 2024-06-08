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
```
### Pre-Increment and Post-Increment
Certainly! Below are explanations and examples for pre-increment, post-increment, pre-decrement, and post-decrement in C++.

### Pre-Increment and Post-Increment

#### Pre-Increment (`++a`)
The pre-increment operator increments the value of the variable by 1 before using it in an expression. 

**Syntax:**
```cpp
++variable;
```

**Example:**
```cpp
#include <iostream>

int main() {
    int a = 5;
    int b = ++a; // First increments a to 6, then assigns 6 to b.
    
    std::cout << "a = " << a << std::endl; // Outputs: a = 6
    std::cout << "b = " << b << std::endl; // Outputs: b = 6
    
    return 0;
}
```

#### Post-Increment (`a++`)
The post-increment operator increments the value of the variable by 1 after using it in an expression.

**Syntax:**
```cpp
variable++;
```

**Example:**
```cpp
#include <iostream>

int main() {
    int a = 5;
    int b = a++; // First assigns 5 to b, then increments a to 6.
    
    std::cout << "a = " << a << std::endl; // Outputs: a = 6
    std::cout << "b = " << b << std::endl; // Outputs: b = 5
    
    return 0;
}
```

#### Pre-Decrement (`--a`)
The pre-decrement operator decrements the value of the variable by 1 before using it in an expression.

**Syntax:**
```cpp
--variable;
```

**Example:**
```cpp
#include <iostream>

int main() {
    int a = 5;
    int b = --a; // First decrements a to 4, then assigns 4 to b.
    
    std::cout << "a = " << a << std::endl; // Outputs: a = 4
    std::cout << "b = " << b << std::endl; // Outputs: b = 4
    
    return 0;
}
```

#### Post-Decrement (`a--`)
The post-decrement operator decrements the value of the variable by 1 after using it in an expression.

**Syntax:**
```cpp
variable--;
```

**Example:**
```cpp
#include <iostream>

int main() {
    int a = 5;
    int b = a--; // First assigns 5 to b, then decrements a to 4.
    
    std::cout << "a = " << a << std::endl; // Outputs: a = 4
    std::cout << "b = " << b << std::endl; // Outputs: b = 5
    
    return 0;
}
```

### Summary
- **Pre-Increment (`++a`)**: Increments the variable before using it.
- **Post-Increment (`a++`)**: Uses the variable, then increments it.
- **Pre-Decrement (`--a`)**: Decrements the variable before using it.
- **Post-Decrement (`a--`)**: Uses the variable, then decrements it.

Each of these operations is essential for controlling the flow of loops and managing state changes in algorithms effectively.
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

```

#include <iostream>

int main() {
    bool a = true, b = false;
    std::cout << "a && b = " << (a && b) << std::endl;
    std::cout << "a || b = " << (a || b) << std::endl;
    std::cout << "!a = " << (!a) << std::endl;
    return 0;
}
```

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


```

#include <iostream>

int main() {
    int a = 5;  // 0101 in binary
    int b = 3;  // 0011 in binary
    std::cout << "a & b = " << (a & b) << std::endl;  // 0001
    std::cout << "a | b = " << (a | b) << std::endl;  // 0111
    std::cout << "a ^ b = " << (a ^ b) << std::endl;  // 0110
    std::cout << "~a = " << (~a) << std::endl;  // 11111111111111111111111111111010 (assuming 32-bit int)
    std::cout << "a << 1 = " << (a << 1) << std::endl;  // 1010
    std::cout << "a >> 1 = " << (a >> 1) << std::endl;  // 0010
    return 0;
}



