### C++ Conditional Statements Syntax and Examples

#### 1. **If Statement**
The `if` statement executes a block of code if a specified condition is true.

**Syntax:**
```cpp
if (condition) {
    // Code to execute if condition is true
}
```

**Example:**
```cpp
#include <iostream>

int main() {
    int age = 20;

    if (age >= 18) {
        std::cout << "You are an adult." << std::endl;
    }

    return 0;
}
```

#### 2. **If-Else Statement**
The `if-else` statement executes one block of code if a condition is true and another block of code if the condition is false.

**Syntax:**
```cpp
if (condition) {
    // Code to execute if condition is true
} else {
    // Code to execute if condition is false
}
```

**Example:**
```cpp
#include <iostream>

int main() {
    int age = 16;

    if (age >= 18) {
        std::cout << "You are an adult." << std::endl;
    } else {
        std::cout << "You are not an adult." << std::endl;
    }

    return 0;
}
```

#### 3. **If-Else If-Else Statement**
The `if-else if-else` statement allows you to check multiple conditions. It executes a block of code as soon as one of the conditions is true.

**Syntax:**
```cpp
if (condition1) {
    // Code to execute if condition1 is true
} else if (condition2) {
    // Code to execute if condition2 is true
} else {
    // Code to execute if none of the conditions are true
}
```

**Example:**
```cpp
#include <iostream>

int main() {
    int score = 85;

    if (score >= 90) {
        std::cout << "Grade: A" << std::endl;
    } else if (score >= 80) {
        std::cout << "Grade: B" << std::endl;
    } else if (score >= 70) {
        std::cout << "Grade: C" << std::endl;
    } else if (score >= 60) {
        std::cout << "Grade: D" << std::endl;
    } else {
        std::cout << "Grade: F" << std::endl;
    }

    return 0;
}
```

#### 4. **Switch Statement**
The `switch` statement selects one of many code blocks to execute based on the value of an expression.

**Syntax:**
```cpp
switch (expression) {
    case value1:
        // Code to execute if expression == value1
        break;
    case value2:
        // Code to execute if expression == value2
        break;
    // You can have any number of case statements
    default:
        // Code to execute if expression doesn't match any case
}
```

**Example:**
```cpp
#include <iostream>

int main() {
    int day = 3;

    switch (day) {
        case 1:
            std::cout << "Monday" << std::endl;
            break;
        case 2:
            std::cout << "Tuesday" << std::endl;
            break;
        case 3:
            std::cout << "Wednesday" << std::endl;
            break;
        case 4:
            std::cout << "Thursday" << std::endl;
            break;
        case 5:
            std::cout << "Friday" << std::endl;
            break;
        case 6:
            std::cout << "Saturday" << std::endl;
            break;
        case 7:
            std::cout << "Sunday" << std::endl;
            break;
        default:
            std::cout << "Invalid day" << std::endl;
            break;
    }

    return 0;
}
```

### Summary
Conditional statements are essential for making decisions in your code based on certain conditions. Here are the main types covered:
- **If Statement**: Executes a block of code if a condition is true.
- **If-Else Statement**: Executes one block of code if a condition is true, and another block if the condition is false.
- **If-Else If-Else Statement**: Checks multiple conditions and executes the corresponding block of code for the first true condition.
- **Switch Statement**: Selects a block of code to execute based on the value of an expression.

These statements help in controlling the flow of the program by allowing different executions based on different conditions.