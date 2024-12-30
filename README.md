**Python Comments**  

Comments in Python are used to make the code more readable and to provide explanations or annotations about the logic or purpose of the code. They are ignored by the Python interpreter during execution.  

### Types of Comments:  
1. **Single-line Comments**:  
   - Start with the `#` symbol.  
   - Example:  
     ```python
     # This is a single-line comment
     print("Hello, World!")
     ```

2. **Multi-line Comments**:  
   - Python does not have a specific syntax for multi-line comments, but triple quotes (`'''` or `"""`) are often used as a workaround.  
   - Example:  
     ```python
     """
     This is a multi-line comment.
     It can span multiple lines.
     """
     print("Hello, World!")
     ```

### Best Practices:
- Use comments to explain *why* something is done, not *what* is done (the code itself shows what is done).  
- Keep comments concise and relevant.  
- Avoid over-commenting trivial code.  
Well-commented code improves maintainability and helps others (and your future self) understand the program.

**Python Variables**  

A variable in Python is a container used to store data values. It acts as a label that points to the memory location where the data is stored. Variables can hold different types of data such as numbers, strings, lists, or more complex structures.

### Key Features of Python Variables:
1. **Dynamic Typing**:  
   - Variables do not require explicit declaration of their type. The type is determined based on the assigned value.  
   - Example:  
     ```python
     x = 10       # Integer
     y = "Hello"  # String
     z = 3.14     # Float
     ```

2. **Variable Naming Rules**:
   - Must start with a letter or an underscore (`_`).
   - Can contain letters, digits, and underscores.
   - Cannot use reserved keywords (e.g., `if`, `for`, `class`).
   - Case-sensitive (`name` and `Name` are different).
**Or**
   -A variable name must start with a letter or the underscore character
   -A variable name cannot start with a number
   -A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
   -Variable names are case-sensitive (age, Age and AGE are three different variables)
   -A variable name cannot be any of the Python keywords.

3. **Assigning Values**:
   - Assignment is done using the `=` operator.
   - Example:  
     ```python
     age = 25
     name = "Alice"
     ```

4. **Multiple Assignments**:
   - Assign multiple variables in a single line.  
     ```python
     a, b, c = 1, 2, 3
     ```

5. **Reassignment**:
   - Variables can be reassigned to new values or even different data types.  
     ```python
     x = 5       # Integer
     x = "Five"  # String
     ```
6. **Case-sensitive**:
name = "Alice"
Name = "Bob"
print(name)  # Output: Alice
print(Name)  # Output: Bob
both name and Name are differtnt variable

**Examples:**
**Valid names:**
myVar, _myVar, var_2

**Invalid names:**
2myVar, my-var, my var

**Python Variable Assignment**

1. **Assign Multiple Values to Multiple Variables**:  
   You can assign multiple values to multiple variables in a single line.  
   Example:  
   ```python
   x, y, z = "Orange", "Banana", "Cherry"
   print(x)  # Output: Orange
   print(y)  # Output: Banana
   print(z)  # Output: Cherry
   ```
   **Note**: The number of variables must match the number of values.

2. **Assign One Value to Multiple Variables**:  
   You can assign the same value to multiple variables in one line.  
   Example:  
   ```python
   x = y = z = "Orange"
   print(x)  # Output: Orange
   print(y)  # Output: Orange
   print(z)  # Output: Orange
   ```

3. **Unpack a Collection**:  
   You can unpack values from collections like lists or tuples into separate variables.  
   Example:  
   ```python
   fruits = ["apple", "banana", "cherry"]
   x, y, z = fruits
   print(x)  # Output: apple
   print(y)  # Output: banana
   print(z)  # Output: cherry
   ```

**Multi-word variable names:**
**Camel Case:** myVariableName
**Pascal Case:** MyVariableName
**Snake Case:** my_variable_name
Python's simplicity and flexibility with variables make it a powerful language for developers.
