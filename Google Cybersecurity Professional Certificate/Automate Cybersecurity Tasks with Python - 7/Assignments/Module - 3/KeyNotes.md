````md
# Key Notes: Python Data Handling for Cybersecurity

---

## 1. Working with Strings

Strings are sequences of characters used to represent text-based data such as usernames, IP addresses, URLs, and device IDs.

### Core Concepts
- Strings are **ordered**, meaning each character has a position called an index.
- Indexing starts at **0**; negative indexing counts from the end.
- Strings are **immutable**, so their values cannot be changed after creation.

### Common Operations
- **Indexing (bracket notation)**: access single characters
  ```python
  device_id = "h32rb17"
  device_id[0]  # 'h'
````

* **Slicing**: extract a portion of a string

  ```python
  device_id[0:3]  # 'h32'
  ```

### Useful Functions and Methods

* `len()` → returns string length
* `str()` → converts data to string
* `.upper()` → converts to uppercase
* `.lower()` → converts to lowercase
* `.index()` → returns position of a character or substring

### Cybersecurity Use Cases

* Parsing logs
* Extracting parts of IPs, emails, or URLs
* Validating usernames and IDs

---

## 2. Working with Lists and Developing Algorithms

Lists are ordered collections used to store multiple values in a single variable. They are widely used for handling security data in bulk.

### Core Concepts

* Lists are **ordered and indexed**
* Indexing starts at **0**
* Lists are **mutable** (can be modified)
* Can store multiple data types

### Accessing and Modifying Lists

* Access elements:

  ```python
  usernames[2]
  ```
* Modify elements:

  ```python
  usernames[1] = "new_user"
  ```

### Slicing Lists

* Extract sublists:

  ```python
  usernames[0:2]
  ```

### Common List Methods

* `.append()` → adds element to end
* `.insert()` → adds element at specific index
* `.remove()` → deletes first occurrence
* `.index()` → finds position of element

### Algorithm Development

* Lists are often used with **loops**

  ```python
  for user in usernames:
      print(user)
  ```
* Used for:

  * Automating repetitive tasks
  * Filtering data
  * Processing logs
  * Detecting anomalies

---

## 3. Regular Expressions (Regex)

Regular expressions are patterns used to search, match, and extract structured data from text.

### Setup

```python
import re
```

### Key Function

* `re.findall()` → returns all matches as a list

### Character Symbols

* `\w` → letters, digits, underscore
* `\d` → digits (0–9)
* `\s` → whitespace
* `.` → any character except newline
* `\.` → literal dot

### Quantifiers

* `+` → one or more occurrences
* `*` → zero or more occurrences
* `{n}` → exact number of occurrences
* `{n,m}` → range of occurrences

### Example

```python
re.findall("\d+", "h32rb17")
```

Output:

```
['32', '17']
```

### Pattern Building

Regex combines symbols to extract structured data:

```python
pattern = "\w+:\s\d+"
```

Breakdown:

* `\w+` → username
* `:` → separator
* `\s` → space
* `\d+` → numeric values

### Cybersecurity Use Cases

* Log analysis
* Extracting IP addresses and usernames
* Detecting patterns in security data
* Filtering and validating input

---

## Summary

* Strings are used for handling individual text values.
* Lists manage collections of data and support automation through loops.
* Regex enables powerful pattern matching for extracting structured information.

Together, these tools form the foundation of data processing and analysis in cybersecurity workflows.

```
```
