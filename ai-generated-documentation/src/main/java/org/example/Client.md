![Capgemini Logo](https://www.capgemini.com/wp-content/themes/capgemini2020/assets/images/logo.svg)

### Make it real.

---
## Client.java Documentation

**1. Overview:**

This Java code defines a `Client` class that interacts with a `Service` object to generate greetings. The `Client` class takes a `Service` object as a constructor parameter and provides a `greeting` method that accepts a name as input and returns a personalized greeting. The greeting is formatted based on the length of the name and whether it's even or odd.

**2. Package/module name:**

org.example

**3. Class/file name:**

Client.java

**4. Detailed Documentation:**

**- Class `Client`:**

   - **Description:** This class encapsulates the logic for generating personalized greetings based on input from a `Service` object.

   - **Constructor `Client(Service service)`:**

     - **Description:** Initializes a new `Client` instance with the provided `Service` object.
     - **Parameters:**
       - `service`: A `Service` object responsible for handling even/odd number checks.
     - **Return Values:** None.

   - **Method `greeting(String name)`:**

     - **Description:** Generates a personalized greeting based on the provided name.
     - **Parameters:**
       - `name`: A string representing the name to be used in the greeting.
     - **Return Values:**
       - A string containing the personalized greeting.
     - **Important Logic:**
       - **Input Validation:** Checks if the `name` parameter is null or empty. If so, throws an `IllegalArgumentException`.
       - **Even/Odd Check:** Calls the `isEven` method of the `service` object to determine if the length of the name is even.
       - **Greeting Formatting:** Formats the greeting string using string interpolation.
       - **Case Sensitivity:** If the name length is even, the greeting is returned in uppercase; otherwise, it's returned in lowercase.

**5. Pseudo Code:**

```
// Class: Client

// Method: greeting(name)
  1. Check if name is null or empty:
    - If true, throw an "IllegalArgumentException" with message "'name' must not be null or empty".
  2. Call service.isEven(name.length()) to check if the length of the name is even.
  3. Format the greeting string using string interpolation: "Hello, %s".formatted(name).
  4. If the length of the name is even:
    - Return the formatted greeting in uppercase.
  5. Else:
    - Return the formatted greeting in lowercase.
```



**Dependencies and Libraries:**

- The code relies on a `Service` class, which is not provided. This class likely contains the `isEven` method.

- **Equivalent Libraries:**

  - **Java:** No specific external libraries are used.
  - **Python:**  No direct equivalent, as the `Service` class is custom.
  - **C++:**  No direct equivalent, as the `Service` class is custom.



