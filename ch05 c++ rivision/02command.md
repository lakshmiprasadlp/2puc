# C++ Comments Guide

Comments are lines in a program that are ignored by the compiler. They are used to add explanations or notes within the code, making it easier to understand for anyone reading it. Comments can be used to explain what the code does, why certain decisions were made, or to temporarily disable parts of the code.

## Types of Comments

### Single-line Comments
Single-line comments start with `//`. Everything following `//` on that line is considered a comment and is ignored by the compiler.

**Example:**
```cpp
#include <iostream>
using namespace std;

int main() {
  // This is a single-line comment
  cout << "Hello World!"; // This comment is at the end of a line of code
  return 0;
}
```

### Multi-line Comments
Multi-line comments start with `/*` and end with `*/`. Everything between `/*` and `*/` is considered a comment and is ignored by the compiler.

**Example:**
```cpp
#include <iostream>
using namespace std;

int main() {
  /* This is a multi-line comment
     that spans multiple lines */
  cout << "Hello World!";
  return 0;
}
```

### Nested Comments
Standard C++ does not support nested comments. Nested comments are comments within comments. While you can nest single-line comments within multi-line comments, you cannot nest multi-line comments within each other.

**Example:**
```cpp
#include <iostream>
using namespace std;

int main() {
  /* This is a multi-line comment
     // This is a single-line comment inside a multi-line comment
     that spans multiple lines */
  cout << "Hello World!";
  return 0;
}
```

**Invalid Nested Comment Example:**
```cpp
#include <iostream>
using namespace std;

int main() {
  /* This is a multi-line comment
     /* This is an attempt to nest another multi-line comment */
     that will cause an error */
  cout << "Hello World!";
  return 0;
}
```

## Best Practices for Using Comments

1. **Keep Comments Relevant and Up-to-date:** Ensure comments accurately reflect the code they describe. Outdated comments can be misleading.
2. **Avoid Obvious Comments:** Don't comment on things that are clear from the code itself. For example:
   ```cpp
   int x = 5; // Set x to 5 (this is obvious and unnecessary)
   ```
3. **Use Comments to Explain Why, Not What:** Comments should explain the reasoning behind certain decisions rather than what the code is doing, which should be clear from the code itself.
   ```cpp
   int x = calculateValue(); // Explain why calculateValue() is called here
   ```
4. **Be Consistent:** Follow a consistent style for comments throughout the codebase.
5. **Use Multi-line Comments for Large Explanations:** When a detailed explanation is required, use multi-line comments to provide clarity.

## Commenting Out Code
You can use comments to temporarily disable parts of your code during debugging or testing.

**Example:**
```cpp
#include <iostream>
using namespace std;

int main() {
  // cout << "This line is commented out and won't be executed";
  cout << "Hello World!";
  return 0;
}
```

By understanding and effectively using comments, you can make your code more readable, maintainable, and easier to understand for yourself and others who may work with your code.