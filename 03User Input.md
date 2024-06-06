# C++ User Input Guide

In C++, user input is typically handled using the `cin` object, which is part of the standard input/output stream library (`<iostream>`). This object is used in conjunction with the extraction operator (`>>`) to read data from the standard input, usually the keyboard.

## Basic User Input

### Example: Reading an Integer
To read an integer input from the user, you can use the following code:
```cpp
#include <iostream>
using namespace std;

int main() {
  int myNum;
  cout << "Enter a number: ";
  cin >> myNum;
  cout << "You entered: " << myNum << endl;
  return 0;
}
```

### Explanation
- **`#include <iostream>`**: Includes the I/O stream library needed for input and output operations.
- **`using namespace std;`**: Allows us to use standard library objects without prefixing them with `std::`.
- **`int myNum;`**: Declares an integer variable `myNum`.
- **`cout << "Enter a number: ";`**: Prompts the user to enter a number.
- **`cin >> myNum;`**: Reads the user input and stores it in `myNum`.
- **`cout << "You entered: " << myNum << endl;`**: Outputs the entered number.

## Reading Multiple Inputs

### Example: Reading Multiple Values
You can read multiple inputs in a single line or separately:
```cpp
#include <iostream>
using namespace std;

int main() {
  int age;
  double height;
  cout << "Enter your age and height: ";
  cin >> age >> height;
  cout << "You entered age: " << age << " and height: " << height << endl;
  return 0;
}
```

### Explanation
- **`cin >> age >> height;`**: Reads two values from the user and stores them in `age` and `height`.

## Reading Strings

### Example: Reading a Single Word
To read a single word string, use `cin`:
```cpp
#include <iostream>
using namespace std;

int main() {
  string name;
  cout << "Enter your name: ";
  cin >> name;
  cout << "Hello, " << name << "!" << endl;
  return 0;
}
```



## Handling Different Data Types

### Example: Reading Different Data Types
You can read various data types using `cin`:
```cpp
#include <iostream>
using namespace std;

int main() {
  int age;
  double salary;
  char grade;

  cout << "Enter your age: ";
  cin >> age;
  cout << "Enter your salary: ";
  cin >> salary;
  cout << "Enter your grade: ";
  cin >> grade;

  cout << "Age: " << age << ", Salary: " << salary << ", Grade: " << grade << endl;
  return 0;
}
```

### Explanation
- **`cin >> age;`**: Reads an integer.
- **`cin >> salary;`**: Reads a double.
- **`cin >> grade;`**: Reads a single character.

