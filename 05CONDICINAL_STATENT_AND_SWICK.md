Sure! Conditional statements in C++ allow the program to take different paths based on certain conditions. The main conditional statements are `if`, `if-else`, `if-else if-else`, and `switch`.

### Syntax

1. **`if` Statement**:
    ```cpp
    if (condition) {
        // code to be executed if the condition is true
    }
    ```

2. **`if-else` Statement**:
    ```cpp
    if (condition) {
        // code to be executed if the condition is true
    } else {
        // code to be executed if the condition is false
    }
    ```

3. **`if-else if-else` Statement**:
    ```cpp
    if (condition1) {
        // code to be executed if condition1 is true
    } else if (condition2) {
        // code to be executed if condition2 is true
    } else {
        // code to be executed if both condition1 and condition2 are false
    }
    ```

4. **`switch` Statement**:
    ```cpp
    switch (expression) {
        case constant1:
            // code to be executed if expression == constant1
            break;
        case constant2:
            // code to be executed if expression == constant2
            break;
        // more cases
        default:
            // code to be executed if expression doesn't match any case
    }
    ```

### Examples

1. **Example using `if` Statement**:
    ```cpp
    #include <iostream>

    int main() {
        int number = 10;

        if (number > 0) {
            std::cout << "The number is positive." << std::endl;
        }

        return 0;
    }
    ```

2. **Example using `if-else` Statement**:
    ```cpp
    #include <iostream>

    int main() {
        int number = -5;

        if (number > 0) {
            std::cout << "The number is positive." << std::endl;
        } else {
            std::cout << "The number is not positive." << std::endl;
        }

        return 0;
    }
    ```

3. **Example using `if-else if-else` Statement**:
    ```cpp
    #include <iostream>

    int main() {
        int number = 0;

        if (number > 0) {
            std::cout << "The number is positive." << std::endl;
        } else if (number < 0) {
            std::cout << "The number is negative." << std::endl;
        } else {
            std::cout << "The number is zero." << std::endl;
        }

        return 0;
    }
    ```

4. **Example using `switch` Statement**:
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
        }

        return 0;
    }
    ```

### Explanation

1. **`if` Statement**: Checks a condition, and if it evaluates to true, the code inside the block is executed.
2. **`if-else` Statement**: Provides an alternative path if the condition is false.
3. **`if-else if-else` Statement**: Allows multiple conditions to be checked in sequence.
4. **`switch` Statement**: Selects one of many code blocks to execute based on the value of an expression. It is often used for menu-driven programs and scenarios with multiple discrete values. 

These examples cover basic conditional constructs in C++, which are fundamental for controlling the flow of a program.