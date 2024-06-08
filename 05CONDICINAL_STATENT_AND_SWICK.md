Certainly! Here are the examples modified to use `cin` for input and `using namespace std;` for simplicity.

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
using namespace std;

int main() {
    int age;
    cout << "Enter your age: ";
    cin >> age;

    if (age >= 18) {
        cout << "You are an adult." << endl;
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
using namespace std;

int main() {
    int age;
    cout << "Enter your age: ";
    cin >> age;

    if (age >= 18) {
        cout << "You are an adult." << endl;
    } else {
        cout << "You are not an adult." << endl;
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
using namespace std;

int main() {
    int score;
    cout << "Enter your score: ";
    cin >> score;

    if (score >= 90) {
        cout << "Grade: A" << endl;
    } else if (score >= 80) {
        cout << "Grade: B" << endl;
    } else if (score >= 70) {
        cout << "Grade: C" << endl;
    } else if (score >= 60) {
        cout << "Grade: D" << endl;
    } else {
        cout << "Grade: F" << endl;
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
using namespace std;

int main() {
    int day;
    cout << "Enter the day of the week (1-7): ";
    cin >> day;

    switch (day) {
        case 1:
            cout << "Monday" << endl;
            break;
        case 2:
            cout << "Tuesday" << endl;
            break;
        case 3:
            cout << "Wednesday" << endl;
            break;
        case 4:
            cout << "Thursday" << endl;
            break;
        case 5:
            cout << "Friday" << endl;
            break;
        case 6:
            cout << "Saturday" << endl;
            break;
        case 7:
            cout << "Sunday" << endl;
            break;
        default:
            cout << "Invalid day" << endl;
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