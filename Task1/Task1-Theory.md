# Section 1 -- Basic Python MCQs (Questions with Answers)

## 1. What is Python?

**Answer:**\
Python is a high-level, interpreted, object-oriented, and
general-purpose programming language known for its simple syntax and
readability.

------------------------------------------------------------------------

## 2. Why is Python so popular?

**Answer:**

-   Easy to learn and read
-   Large standard library
-   Huge community support
-   Cross-platform
-   Open-source
-   Supports multiple programming paradigms
-   Used in AI, ML, Web Development, Automation, Data Science,
    Cybersecurity, etc.

------------------------------------------------------------------------

## 3. Why is Python preferred for AI/ML?

**Answer:**

-   Simple syntax
-   Extensive AI/ML libraries (NumPy, Pandas, Scikit-learn, TensorFlow,
    PyTorch)
-   Large community
-   Faster prototyping
-   Strong visualization support
-   Easy integration with C/C++

------------------------------------------------------------------------

## 4. Which of the following is an interpreted language?

**Answer:** Python.

------------------------------------------------------------------------

## 5. Which of the following is dynamically typed?

**Answer:** Python.

------------------------------------------------------------------------

## 6. Difference between Python 2 and Python 3?

  Python 2                     Python 3
  ---------------------------- -------------------------
  Older version                Latest version
  `print` is a statement       `print()` is a function
  `xrange()`                   `range()`
  Unicode support is limited   Unicode by default
  No longer supported          Actively supported

------------------------------------------------------------------------

## 7. Which version is currently recommended?

**Answer:** Python 3.

------------------------------------------------------------------------

## 8. What is the output of `print(type(10))`?

``` python
print(type(10))
```

**Output**

``` python
<class 'int'>
```

------------------------------------------------------------------------

## 9. What is the output of `print(type(10.5))`?

``` python
print(type(10.5))
```

**Output**

``` python
<class 'float'>
```

------------------------------------------------------------------------

## 10. Which data types are immutable?

-   `int`
-   `float`
-   `bool`
-   `str`
-   `tuple`
-   `frozenset`
-   `bytes`

------------------------------------------------------------------------

## 11. Which data types are mutable?

-   `list`
-   `dict`
-   `set`
-   `bytearray`

------------------------------------------------------------------------

## 12. Exponentiation operator

`**`

Example:

``` python
2 ** 3
# Output: 8
```

------------------------------------------------------------------------

## 13. Difference between `==` and `is`

  `==`              `is`
  ----------------- --------------------------
  Compares values   Compares object identity

``` python
a = [1,2]
b = [1,2]

a == b   # True
a is b   # False
```

------------------------------------------------------------------------

## 14. Difference between `and` and `&`

  `and`              `&`
  ------------------ ------------------
  Logical operator   Bitwise operator
  Short-circuit      No short-circuit

``` python
True and False   # False
5 & 3            # 1
```

------------------------------------------------------------------------

## 15. Difference between `/` and `//`

  `/`              `//`
  ---------------- ----------------
  Float division   Floor division

``` python
7 / 2    # 3.5
7 // 2   # 3
```

------------------------------------------------------------------------

## 16. Difference between `%` and `divmod()`

  `%`                 `divmod()`
  ------------------- --------------------------------
  Returns remainder   Returns quotient and remainder

``` python
10 % 3          # 1
divmod(10,3)    # (3, 1)
```

------------------------------------------------------------------------

## 17. Membership operators

-   `in`
-   `not in`

``` python
"a" in "apple"   # True
```

------------------------------------------------------------------------

## 18. Identity operators

-   `is`
-   `is not`

------------------------------------------------------------------------

## 19. Implicit type casting

Automatic conversion by Python.

``` python
5 + 2.5   # 7.5
```

------------------------------------------------------------------------

## 20. Explicit type casting

Manual conversion using functions.

``` python
int("10")   # 10
```

------------------------------------------------------------------------

## 21. String to integer

`int()`

------------------------------------------------------------------------

## 22. Integer to string

`str()`

------------------------------------------------------------------------

## 23. Function to get data type

`type()`

------------------------------------------------------------------------

## 24. Function to get object identity

`id()`

------------------------------------------------------------------------

## 25. `bool("")`

``` python
False
```

------------------------------------------------------------------------

## 26. `bool([])`

``` python
False
```

------------------------------------------------------------------------

## 27. `bool(None)`

``` python
False
```

------------------------------------------------------------------------

## 28. False values in Python

-   `False`
-   `None`
-   `0`
-   `0.0`
-   `0j`
-   `""`
-   `''`
-   `[]`
-   `{}`
-   `()`
-   `set()`
-   `range(0)`

Everything else is `True`.

------------------------------------------------------------------------

## 29. What is PEP 8?

PEP 8 (Python Enhancement Proposal 8) is the official Python style guide
for writing clean, readable, and consistent code.

------------------------------------------------------------------------

## 30. Why is indentation important?

Indentation defines code blocks in Python. Incorrect indentation causes
an `IndentationError` or changes program logic.

------------------------------------------------------------------------

**End of Section 1 -- Basic Python MCQs**
