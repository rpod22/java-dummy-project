![Capgemini Logo](https://www.capgemini.com/wp-content/themes/capgemini2020/assets/images/logo.svg)

### Make it real.

---
## Service.java Documentation

**1. Overview:**

This Java code defines a `Service` class that provides utility methods for basic mathematical operations and conditional logic. It includes a method to check if a number is even and a more complex method that analyzes the signs of three integers.

**2. Package/module name:**

org.example

**3. Class/file name:**

Service.java

**4. Detailed Documentation:**

**- Class `Service`:**

   - **Description:** This class encapsulates utility methods for checking even numbers and analyzing the signs of integers.

   - **Method `isEven(int input)`:**

     - **Description:** Determines if a given integer is even.
     - **Parameters:**
       - `input`: An integer to be checked.
     - **Return Values:**
       - `true` if the input is even, `false` otherwise.
     - **Important Logic:**
       - Uses the modulo operator (`%`) to check if the remainder of the input divided by 2 is 0.

   - **Method `highComplexityMethod(int a, int b, int c)`:**

     - **Description:** Analyzes the signs of three integers (`a`, `b`, and `c`) and prints messages based on their combinations.
     - **Parameters:**
       - `a`: The first integer.
       - `b`: The second integer.
       - `c`: The third integer.
     - **Return Values:**
       - None.
     - **Important Logic:**
       - Uses nested `if` statements to check the signs of `a`, `b`, and `c` in all possible combinations.
       - Prints messages indicating the signs of each integer and their relationships.

**5. Pseudo Code:**

```
// Class: Service

// Method: isEven(input)
  1. Calculate the remainder when input is divided by 2.
  2. If the remainder is 0, return true.
  3. Otherwise, return false.

// Method: highComplexityMethod(a, b, c)
  1. Check the sign of a:
    - If a is positive:
      - Check the sign of b:
        - If b is positive:
          - Check the sign of c:
            - If c is positive, print "a, b, and c are positive".
            - If c is non-positive, print "a and b are positive, c is non-positive".
        - If b is non-positive:
          - Check the sign of c:
            - If c is positive, print "a is positive, b and c are non-positive".
            - If c is non-positive, print "a and b are non-positive, c is non-positive".
    - If a is non-positive:
      - Check the sign of b:
        - If b is positive:
          - Check the sign of c:
            - If c is positive, print "a is non-positive, b and c are positive".
            - If c is non-positive, print "a is non-positive, b is positive, c is non-positive".
        - If b is non-positive:
          - Check the sign of c:
            - If c is positive, print "a and b are non-positive, c is positive".
            - If c is non-positive, print "a and b are non-positive, c is non-positive".



```



**Dependencies and Libraries:**

- This code does not rely on any external libraries.



