# Introduction to Python Programming in Cybersecurity

## What is Python?
- Python is a high-level, interpreted programming language.
- Known for its simple syntax and readability.
- Widely used in cybersecurity, automation, data analysis, and scripting.

## Importance of Python in Cybersecurity
- Automates repetitive security tasks.
- Processes and analyzes large volumes of security data.
- Supports incident response and threat detection.
- Helps manage logs, user accounts, and system configurations.
- Integrates with security tools and APIs.

## Common Cybersecurity Applications
- Log analysis
- Network monitoring
- Vulnerability scanning
- Threat intelligence gathering
- Security automation
- Incident response scripting

## Python Development Environments
### Notebooks
- Interactive environments for writing and executing code.
- Support code cells and markdown cells.
- Examples:
  - Jupyter Notebook
  - Google Colab

### Integrated Development Environments (IDEs)
- Software applications for coding and debugging.
- Provide syntax highlighting and error detection.
- Examples:
  - Visual Studio Code
  - PyCharm

### Command Line Interface (CLI)
- Text-based environment for running Python scripts.
- Useful for automation and system administration.

---

# Core Python Components

## Variables
- Named containers used to store data.
- Values can be updated during program execution.

### Example
```python
username = "admin"
```

## Data Types

### String (str)
- Stores text data.
```python
username = "admin"
```

### Integer (int)
- Stores whole numbers.
```python
attempts = 5
```

### Float (float)
- Stores decimal values.
```python
score = 98.5
```

### Boolean (bool)
- Represents True or False values.
```python
logged_in = True
```

## Comments
- Used to explain code.
- Ignored during execution.

```python
# This is a comment
```

## Functions
- Reusable blocks of code that perform specific tasks.

### Built-in Function Example
```python
print("Hello")
```

## Operators

### Arithmetic Operators
| Operator | Purpose |
|-----------|---------|
| + | Addition |
| - | Subtraction |
| * | Multiplication |
| / | Division |
| % | Modulus |

### Comparison Operators
| Operator | Purpose |
|-----------|---------|
| == | Equal to |
| != | Not equal to |
| > | Greater than |
| < | Less than |
| >= | Greater than or equal to |
| <= | Less than or equal to |

### Logical Operators
| Operator | Purpose |
|-----------|---------|
| and | Both conditions must be true |
| or | At least one condition must be true |
| not | Reverses a condition |

## Lists
- Ordered collections of data.

```python
users = ["alice", "bob", "charlie"]
```

## Strings and Indexing
- Strings are sequences of characters.
- Characters can be accessed using indexes.

```python
word = "security"
print(word[0])
```

---

# Conditional and Iterative Statements

## Conditional Statements

### Purpose
- Allow programs to make decisions based on conditions.

### if Statement
Executes code when a condition is true.

```python
if status == 200:
    print("OK")
```

### else Statement
Executes when the previous condition is false.

```python
if status == 200:
    print("OK")
else:
    print("Error")
```

### elif Statement
Checks additional conditions.

```python
if status == 200:
    print("OK")
elif status == 400:
    print("Bad Request")
else:
    print("Other Status")
```

## Logical Operators in Conditions

### and
Both conditions must be true.

```python
if status >= 200 and status <= 226:
    print("Success")
```

### or
At least one condition must be true.

```python
if status == 100 or status == 102:
    print("Informational")
```

### not
Reverses a condition.

```python
if not(status == 200):
    print("Check status")
```

---

# Iterative Statements (Loops)

## Purpose
- Repeat a block of code multiple times.

## for Loop
Used to iterate through sequences.

### List Example
```python
users = ["alice", "bob", "charlie"]

for user in users:
    print(user)
```

### String Example
```python
for letter in "security":
    print(letter)
```

## range() Function
Generates a sequence of numbers.

```python
for i in range(5):
    print(i)
```

Output:
0, 1, 2, 3, 4

## while Loop
Repeats while a condition remains true.

```python
count = 0

while count < 5:
    print(count)
    count += 1
```

## Loop Control Statements

### break
Stops the loop immediately.

```python
for asset in assets:
    if asset == "desktop20":
        break
```

### continue
Skips the current iteration.

```python
for asset in assets:
    if asset == "desktop20":
        continue
```

## Infinite Loops
- Occur when a loop never reaches a stopping condition.
- Usually caused by incorrect logic or missing updates to loop variables.

```python
while True:
    print("Running...")
```

---

# Quick Revision Points

- Python is widely used for cybersecurity automation and analysis.
- Variables store data and can be reassigned.
- Common data types: String, Integer, Float, Boolean.
- Functions allow code reuse.
- Conditional statements: `if`, `elif`, `else`.
- Logical operators: `and`, `or`, `not`.
- `for` loops iterate through sequences.
- `while` loops iterate based on conditions.
- `break` exits a loop.
- `continue` skips the current iteration.
- Proper indentation is essential in Python.