Boolean algebra is a branch of algebra that deals with true or false values, typically represented as 1 (true) and 0 (false). It's foundational for digital logic and computer science, involving operations like AND, OR, NOT, and XOR. Let's cover the basic operations:

1. **AND Operation (⋅):**
   - \( A \cdot B \) (or \( A \text{ AND } B \)) is true if both A and B are true.
   - Truth Table:
     | A | B | A ⋅ B |
     |---|---|-------|
     | 0 | 0 |   0   |
     | 0 | 1 |   0   |
     | 1 | 0 |   0   |
     | 1 | 1 |   1   |

2. **OR Operation (+):**
   - \( A + B \) (or \( A \text{ OR } B \)) is true if at least one of A or B is true.
   - Truth Table:
     | A | B | A + B |
     |---|---|-------|
     | 0 | 0 |   0   |
     | 0 | 1 |   1   |
     | 1 | 0 |   1   |
     | 1 | 1 |   1   |

3. **NOT Operation (¯):**
   - \( \overline{A} \) (or NOT A) is true if A is false.
   - Truth Table:
     | A | ¯A |
     |---|----|
     | 0 | 1  |
     | 1 | 0  |

4. **XOR Operation (⊕):**
   - \( A \oplus B \) (or \( A \text{ XOR } B \)) is true if A and B are different.
   - Truth Table:
     | A | B | A ⊕ B |
     |---|---|-------|
     | 0 | 0 |   0   |
     | 0 | 1 |   1   |
     | 1 | 0 |   1   |
     | 1 | 1 |   0   |

### Laws and Properties of Boolean Algebra

1. **Identity Laws:**
   - \( A + 0 = A \)
   - \( A \cdot 1 = A \)

2. **Null Laws:**
   - \( A + 1 = 1 \)
   - \( A \cdot 0 = 0 \)

3. **Idempotent Laws:**
   - \( A + A = A \)
   - \( A \cdot A = A \)

4. **Complement Laws:**
   - \( A + \overline{A} = 1 \)
   - \( A \cdot \overline{A} = 0 \)

5. **Commutative Laws:**
   - \( A + B = B + A \)
   - \( A \cdot B = B \cdot A \)

6. **Associative Laws:**
   - \( (A + B) + C = A + (B + C) \)
   - \( (A \cdot B) \cdot C = A \cdot (B \cdot C) \)

7. **Distributive Laws:**
   - \( A \cdot (B + C) = (A \cdot B) + (A \cdot C) \)
   - \( A + (B \cdot C) = (A + B) \cdot (A + C) \)

8. **De Morgan's Theorems:**
   - \( \overline{A + B} = \overline{A} \cdot \overline{B} \)
   - \( \overline{A \cdot B} = \overline{A} + \overline{B} \)

### Example of Simplifying a Boolean Expression

Let's simplify the Boolean expression \( A \cdot (\overline{A} + B) \):

1. Apply the Distributive Law:
   \( A \cdot (\overline{A} + B) = (A \cdot \overline{A}) + (A \cdot B) \)

2. Apply the Complement Law:
   \( (A \cdot \overline{A}) + (A \cdot B) = 0 + (A \cdot B) \)

3. Apply the Identity Law:
   \( 0 + (A \cdot B) = A \cdot B \)

Thus, \( A \cdot (\overline{A} + B) = A \cdot B \).








#include <iostream>

int main() {
    int a = 5;
    int b = 10;

    // Equal to
    std::cout << (a == b ? "a is equal to b" : "a is not equal to b") << std::endl;

    // Not equal to
    std::cout << (a != b ? "a is not equal to b" : "a is equal to b") << std::endl;

    // Greater than
    std::cout << (a > b ? "a is greater than b" : "a is not greater than b") << std::endl;

    // Less than
    std::cout << (a < b ? "a is less than b" : "a is not less than b") << std::endl;

    // Greater than or equal to
    std::cout << (a >= b ? "a is greater than or equal to b" : "a is not greater than or equal to b") << std::endl;

    // Less than or equal to
    std::cout << (a <= b ? "a is less than or equal to b" : "a is not less than or equal to b") << std::endl;

    return 0;
}
