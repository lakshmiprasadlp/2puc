### Loops in C++

Loops are used in programming to execute a block of code repeatedly as long as a specified condition is met. C++ supports several types of loops: `for`, `while`, and `do-while`.

#### 1. **For Loop**
The `for` loop is typically used when the number of iterations is known beforehand.

**Syntax:**
```cpp
for (initialization; condition; increment) {
    // Code to execute in each iteration
}
```

**Example 1: Print numbers from 1 to 10**

**Use Case**: Iterating over a range of numbers
```cpp
#include <iostream>
using namespace std;

int main() {
    for (int i = 1; i <= 10; i++) {
        cout << i << " ";
    }
    cout << endl;
    return 0;
}
```

**Example 2: Calculate the sum of the first N natural numbers**

**Use Case**: Summing a series of numbers
```cpp
#include <iostream>
using namespace std;

int main() {
    int n, sum = 0;
    cout << "Enter a positive integer: ";
    cin >> n;

    for (int i = 1; i <= n; i++) {
        sum += i;
    }

    cout << "Sum of the first " << n << " natural numbers is " << sum << endl;
    return 0;
}
```

#### 2. **While Loop**
The `while` loop is used when the number of iterations is not known beforehand and depends on a condition.

**Syntax:**
```cpp
while (condition) {
    // Code to execute as long as the condition is true
}
```

**Example 1: Print numbers from 1 to 10**

**Use Case**: Iterating until a condition is false
```cpp
#include <iostream>
using namespace std;

int main() {
    int i = 1;
    while (i <= 10) {
        cout << i << " ";
        i++;
    }
    cout << endl;
    return 0;
}
```

**Example 2: Find the factorial of a number**

**Use Case**: Calculating factorial where the number of iterations depends on the input
```cpp
#include <iostream>
using namespace std;

int main() {
    int n, factorial = 1;
    cout << "Enter a positive integer: ";
    cin >> n;

    int i = n;
    while (i > 0) {
        factorial *= i;
        i--;
    }

    cout << "Factorial of " << n << " is " << factorial << endl;
    return 0;
}
```

#### 3. **Do-While Loop**
The `do-while` loop is similar to the `while` loop, but it guarantees that the loop body is executed at least once.

**Syntax:**
```cpp
do {
    // Code to execute
} while (condition);
```

**Example 1: Print numbers from 1 to 10**

**Use Case**: Ensuring the loop body is executed at least once
```cpp
#include <iostream>
using namespace std;

int main() {
    int i = 1;
    do {
        cout << i << " ";
        i++;
    } while (i <= 10);
    cout << endl;
    return 0;
}
```

**Example 2: Prompt user to enter a positive number**

**Use Case**: Validating user input
```cpp
#include <iostream>
using namespace std;

int main() {
    int number;
    do {
        cout << "Enter a positive number: ";
        cin >> number;
    } while (number <= 0);

    cout << "You entered " << number << endl;
    return 0;
}
```

### Summary
Loops are fundamental in programming for repeating a block of code multiple times. The choice of loop (`for`, `while`, `do-while`) depends on the specific use case and whether the number of iterations is known beforehand. Here are the main types:
- **For Loop**: Best when the number of iterations is known.
- **While Loop**: Best when the number of iterations is unknown and depends on a condition.
- **Do-While Loop**: Best when the loop body must be executed at least once before checking the condition.


