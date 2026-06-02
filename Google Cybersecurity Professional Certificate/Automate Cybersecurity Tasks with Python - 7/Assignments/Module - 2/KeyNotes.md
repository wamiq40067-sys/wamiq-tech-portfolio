# Key Notes: Introduction to Functions, Work with Functions, and Learn from the Python Community

---

# 1. Introduction to Functions

## What is a Function?
- A function is a reusable block of code that performs a specific task.
- Functions help reduce repetition and improve code organization.
- They make programs easier to read, maintain, and debug.

## Importance of Functions
- Promote code reusability.
- Reduce duplication of code.
- Improve readability and maintainability.
- Simplify complex programs by breaking them into smaller tasks.

## Types of Functions

### Built-in Functions
- Functions that come pre-installed with Python.
- Can be used directly without defining them.

**Examples:**
```python
print()
len()
max()
min()
sorted()
```

### User-Defined Functions
- Functions created by programmers to meet specific requirements.

**Example:**
```python
def display_message():
    print("Investigate activity")
```

## Function Structure

### Function Header
- Begins with the `def` keyword.
- Contains the function name and parentheses.
- Ends with a colon (`:`).

```python
def function_name():
```

### Function Body
- Contains the code executed when the function is called.
- Must be indented properly.

```python
def display_message():
    print("Investigate activity")
```

## Calling a Function

```python
display_message()
```

## Benefits in Cybersecurity
- Automate repetitive security tasks.
- Analyze multiple log files efficiently.
- Reuse code for monitoring and incident response activities.

---

# 2. Work with Functions

## Parameters and Arguments

### Parameters
- Variables defined in a function header.
- Receive values when the function is called.

```python
def login_attempts(max_attempts, used_attempts):
```

### Arguments
- Actual values passed to a function.

```python
login_attempts(5, 2)
```

## Return Statements

### Purpose
- Send information back from a function.
- Use the `return` keyword.

```python
def remaining_attempts(max_attempts, used_attempts):
    return max_attempts - used_attempts
```

### Storing Returned Values

```python
remaining = remaining_attempts(5, 2)
```

## Variable Scope

### Global Variables
- Defined outside functions.
- Accessible throughout the program.

```python
username = "admin"
```

### Local Variables
- Defined inside functions.
- Accessible only within the function.

```python
def greet(name):
    message = "Welcome " + name
    return message
```

## Common Built-in Functions

### `max()`
- Returns the largest value.

```python
max([10, 25, 5])
```

### `min()`
- Returns the smallest value.

```python
min([10, 25, 5])
```

### `sorted()`
- Returns a sorted version of an iterable.

```python
sorted([10, 25, 5])
```

## Python Standard Library

### Definition
- A collection of built-in modules included with Python.

### Common Modules

| Module | Purpose |
|----------|---------|
| re | Pattern matching and regular expressions |
| csv | Working with CSV files |
| os | Operating system interaction |
| glob | File searching |
| datetime | Date and time operations |
| statistics | Statistical calculations |

### Importing a Module

```python
import statistics
```

### Importing Specific Functions

```python
from statistics import mean, median
```

## External Libraries

### Definition
- Libraries created by the Python community.
- Must be installed separately.

### Examples
- NumPy
- Beautiful Soup (bs4)
- Pandas
- Matplotlib

### Installation

```python
%pip install numpy
```

### Importing

```python
import numpy
```

---

# 3. Learn from the Python Community

## Python Style Guides

### What is a Style Guide?
- A set of recommendations for writing clean and consistent code.

### PEP 8 Style Guide
- Official Python coding style guide.
- Encourages readability and consistency.

## Comments

### Purpose
- Explain code behavior and programmer intent.
- Improve maintainability.

### Single-Line Comments

```python
# Print all devices
```

### Multi-Line Comments

```python
# Function calculates remaining login attempts
# based on maximum and used attempts.
```

### Docstrings

```python
"""
Calculates remaining login attempts.
Returns an integer value.
"""
```

## Indentation

### Importance
- Defines code blocks in Python.
- Required for correct execution.

### Recommended Standard
- Four spaces per indentation level.

```python
if login_status:
    print("Access granted")
```

## Syntax Best Practices

### Strings
```python
username = "admin"
```

### Numbers
```python
attempts = 5
```

### Booleans
```python
login_status = True
```

### Lists
```python
users = ["admin", "user1"]
```

### Colons
- Required after:
  - Function definitions
  - Loops
  - Conditional statements

```python
def greet():
    pass
```

## Benefits of Community Standards
- Makes code easier to understand.
- Improves collaboration.
- Reduces programming errors.
- Helps create professional-quality code.

---

# Key Takeaways

- Functions are reusable blocks of code that automate tasks.
- Functions consist of headers, parameters, and bodies.
- Arguments provide values to parameters when functions are called.
- Return statements send results back from functions.
- Variables can be global or local depending on scope.
- Built-in functions such as `max()`, `min()`, and `sorted()` simplify data processing.
- The Python Standard Library provides modules for common programming tasks.
- External libraries extend Python's capabilities.
- Comments and docstrings improve code readability.
- PEP 8 provides guidelines for writing clean Python code.
- Proper indentation and syntax are essential for correct program execution.
- Following community standards results in more maintainable and professional code.
```**