# C++ Variables Guide

## Overview
Variables are containers for storing data values. In C++, different types of variables are defined using different keywords.

### Types of Variables
- **int**: Stores integers (whole numbers), without decimals, such as 123 or -123.
- **double**: Stores floating-point numbers, with decimals, such as 19.99 or -19.99.
- **char**: Stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes.
- **string**: Stores text, such as "Hello World". String values are surrounded by double quotes.
- **bool**: Stores values with two states: true or false.

### Declaring Variables
To create a variable, specify the type and assign it a value:
```cpp
type variableName = value;
```
Where `type` is one of the C++ types (such as `int`), and `variableName` is the name of the variable (such as `x` or `myName`).

#### Examples
Create a variable called `myNum` of type `int` and assign it the value 15:
```cpp
int myNum = 15;
cout << myNum;
```

You can also declare a variable without assigning a value initially, and assign the value later:
```cpp
int myNum;
myNum = 15;
cout << myNum;
```

If you assign a new value to an existing variable, it will overwrite the previous value:
```cpp
int myNum = 15;  // myNum is 15
myNum = 10;  // Now myNum is 10
cout << myNum;  // Outputs 10
```

### Other Types
A demonstration of other data types:
```cpp
int myNum = 5;               // Integer
double myFloatNum = 5.99;    // Floating point number
char myLetter = 'D';         // Character
string myText = "Hello";     // String
bool myBoolean = true;       // Boolean
```

### Display Variables
The `cout` object is used together with the `<<` operator to display variables:
```cpp
int myAge = 35;
cout << "I am " << myAge << " years old.";
```

### Add Variables Together
To add a variable to another variable, you can use the `+` operator:
```cpp
int x = 5;
int y = 6;
int sum = x + y;
cout << sum;
```

### Declare Many Variables
To declare more than one variable of the same type, use a comma-separated list:
```cpp
int x = 5, y = 6, z = 50;
cout << x + y + z;
```

### One Value to Multiple Variables
You can also assign the same value to multiple variables in one line:
```cpp
int x, y, z;
x = y = z = 50;
cout << x + y + z;
```

### C++ Identifiers
All C++ variables must be identified with unique names. These unique names are called identifiers.

#### General Rules for Naming Variables
- Names can contain letters, digits, and underscores.
- Names must begin with a letter or an underscore (_).
- Names are case-sensitive (e.g., `myVar` and `myvar` are different variables).
- Names cannot contain whitespaces or special characters like !, #, %, etc.
- Reserved words (like C++ keywords, such as `int`) cannot be used as names.

#### Examples
```cpp
// Good
int minutesPerHour = 60;

// OK, but not so easy to understand what m actually is
int m = 60;
```

### Constants
When you do not want others (or yourself) to change existing variable values, use the `const` keyword. This declares the variable as "constant", which means unchangeable and read-only:
```cpp
const int myNum = 15;  // myNum will always be 15
myNum = 10;  // error: assignment of read-only variable 'myNum'
```

#### Notes on Constants
When you declare a constant variable, it must be assigned with a value:
```cpp
const int minutesPerHour = 60;
```
This, however, will not work:
```cpp
const int minutesPerHour;
minutesPerHour = 60; // error
```