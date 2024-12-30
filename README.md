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
   - A variable name must start with a letter or the underscore character
   - A variable name cannot start with a number
   - A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
   - Variable names are case-sensitive (age, Age and AGE are three different variables)
   - A variable name cannot be any of the Python keywords.

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

**Multi-word variable names:**

**Camel Case:** myVariableName

**Pascal Case:** MyVariableName

**Snake Case:** my_variable_name

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
   **Python Output Variables**

In Python, the `print()` function is used to output variables to the console.

### Examples:

1. **Output a single variable**:
   ```python
   x = "Python is awesome"
   print(x)
   ```

2. **Output multiple variables with commas**:
   ```python
   x = "Python"
   y = "is"
   z = "awesome"
   print(x, y, z)  # Output: Python is awesome
   ```

3. **Output multiple variables using `+`**:
   ```python
   x = "Python "
   y = "is "
   z = "awesome"
   print(x + y + z)  # Output: Python is awesome
   ```

4. **For numbers, `+` works as a mathematical operator**:
   ```python
   x = 5
   y = 10
   print(x + y)  # Output: 15
   ```

5. **Combining string and number with `+` causes an error**:
   ```python
   x = 5
   y = "John"
   print(x + y)  # Error
   ```

**Best Practice**: Use commas to output different types of variables together, as it handles both strings and numbers without errors:
```python
x = 5
y = "John"
print(x, y)  # Output: 5 John
```
   **Global Variables in Python**

Global variables are those defined outside of any function. They can be accessed both inside and outside functions.

### Example:
```python
x = "awesome"  # Global variable

def myfunc():
    print("Python is " + x)  # Accessing global variable inside function

myfunc()  # Output: Python is awesome
```

If you create a variable inside a function with the same name as a global variable, it becomes **local** to that function, and does not affect the global variable.

### Example:
```python
x = "awesome"  # Global variable

def myfunc():
    x = "fantastic"  # Local variable
    print("Python is " + x)  # Output: Python is fantastic

myfunc()

print("Python is " + x)  # Output: Python is awesome
```

In this example, the global variable `x` remains unchanged outside the function, even though the function uses a local `x`.

**Python Built-in Data Types**

Python provides various built-in data types categorized as follows:

### **Data Type Categories**
1. **Text Type**:  
   - `str`: String (e.g., `"Hello"`).

2. **Numeric Types**:  
   - `int`: Integer (e.g., `20`).  
   - `float`: Decimal (e.g., `20.5`).  
   - `complex`: Complex number (e.g., `1j`).

3. **Sequence Types**:  
   - `list`: Ordered, mutable collection (e.g., `["apple", "banana"]`).  
   - `tuple`: Ordered, immutable collection (e.g., `("apple", "banana")`).  
   - `range`: Sequence of numbers (e.g., `range(6)`).

4. **Mapping Type**:  
   - `dict`: Key-value pairs (e.g., `{"name": "John"}`).

5. **Set Types**:  
   - `set`: Unordered, unique items (e.g., `{"apple", "banana"}`).  
   - `frozenset`: Immutable set (e.g., `frozenset({"apple", "banana"})`).

6. **Boolean Type**:  
   - `bool`: Logical values `True` or `False`.

7. **Binary Types**:  
   - `bytes`: Immutable binary data (e.g., `b"Hello"`).  
   - `bytearray`: Mutable binary data (e.g., `bytearray(5)`).  
   - `memoryview`: View of binary data (e.g., `memoryview(bytes(5))`).

8. **None Type**:  
   - `NoneType`: Represents "no value" (e.g., `None`).
# Examples of Python Data Types

Here are examples of different Python data types using built-in functions:

```python
# Text Type
x = str("Hello World")       # str
print(x, type(x))            # Output: Hello World <class 'str'>

# Numeric Types
x = int(20)                  # int
print(x, type(x))            # Output: 20 <class 'int'>

x = float(20.5)              # float
print(x, type(x))            # Output: 20.5 <class 'float'>

x = complex(1j)              # complex
print(x, type(x))            # Output: 1j <class 'complex'>

# Sequence Types
x = list(("apple", "banana", "cherry"))  # list
print(x, type(x))            # Output: ['apple', 'banana', 'cherry'] <class 'list'>

x = tuple(("apple", "banana", "cherry"))  # tuple
print(x, type(x))            # Output: ('apple', 'banana', 'cherry') <class 'tuple'>

x = range(6)                 # range
print(x, type(x))            # Output: range(0, 6) <class 'range'>

# Mapping Type
x = dict(name="John", age=36)  # dict
print(x, type(x))            # Output: {'name': 'John', 'age': 36} <class 'dict'>

# Set Types
x = set(("apple", "banana", "cherry"))  # set
print(x, type(x))            # Output: {'apple', 'banana', 'cherry'} <class 'set'>

x = frozenset(("apple", "banana", "cherry"))  # frozenset
print(x, type(x))            # Output: frozenset({'apple', 'banana', 'cherry'}) <class 'frozenset'>

# Boolean Type
x = bool(5)                  # bool
print(x, type(x))            # Output: True <class 'bool'>

# Binary Types
x = bytes(5)                 # bytes
print(x, type(x))            # Output: b'\x00\x00\x00\x00\x00' <class 'bytes'>

x = bytearray(5)             # bytearray
print(x, type(x))            # Output: bytearray(b'\x00\x00\x00\x00\x00') <class 'bytearray'>

x = memoryview(bytes(5))     # memoryview
print(x, type(x))            # Output: <memory at 0x...> <class 'memoryview'>

# Python has three numeric types:

int - Integer numbers (e.g., 1, 100, -10)
float - Decimal or floating-point numbers (e.g., 1.5, -3.14, 2.0)
complex - Complex numbers with real and imaginary parts (e.g., 3 + 5j, -2j)

