# Topic 2: Variables & Data Types

## 1. What are variables?

**Answer:** A variable is a named memory location used to store data.

Example:

``` python
age = 22
```

## 2. Explain Dynamic Typing.

**Answer:** Python automatically determines a variable's data type at
runtime.

``` python
x = 10
x = "Hello"
```

## 3. Explain Multiple Assignment.

**Answer:** Assign multiple values in one statement.

``` python
a, b, c = 10, 20, 30
x = y = z = 100
a, b = b, a
```

## 4. Explain Variable Naming Conventions.

-   Start with a letter or `_`
-   Cannot start with a digit
-   Use letters, digits and `_`
-   Case-sensitive
-   Cannot use keywords
-   Follow PEP-8 `snake_case`

## 5. Explain Numbers.

Types: - int - float - complex

## 6. Explain Strings.

Strings are ordered, immutable sequences of Unicode characters.

## 7. Explain Lists.

Lists are ordered, mutable collections that allow duplicates.

## 8. Explain Tuples.

Tuples are ordered, immutable collections that allow duplicates.

## 9. Explain Sets.

Sets are unordered, mutable collections of unique elements.

## 10. Explain Dictionaries.

Dictionaries store key-value pairs.

## 11. Difference between List and Tuple.

  List      Tuple
  --------- -----------
  Mutable   Immutable
  \[\]      ()
  Slower    Faster

## 12. Difference between List and Set.

  List         Set
  ------------ ---------------
  Ordered      Unordered
  Duplicates   No duplicates

## 13. Difference between Tuple and Set.

  Tuple       Set
  ----------- -----------
  Ordered     Unordered
  Immutable   Mutable

## 14. Difference between Dictionary and List.

  Dictionary      List
  --------------- -----------------
  Key-value       Values
  Access by key   Access by index

## 15. Difference between Mutable and Immutable Objects.

  Mutable      Immutable
  ------------ ---------------
  Can change   Cannot change

Examples: - Mutable: list, dict, set - Immutable: int, float, str, tuple

## 16. Why are Tuples Immutable?

-   Safety
-   Performance
-   Hashable
-   Can be dictionary keys

## 17. Why are Strings Immutable?

-   Safe
-   Hashable
-   Memory optimization
-   Thread-safe

## 18. Can Dictionary Keys be Mutable?

**No.** Keys must be immutable and hashable.

### Quick Revision

-   Variable: Named container.
-   Dynamic Typing: Type decided at runtime.
-   Multiple Assignment: Multiple variables in one statement.
-   Numbers: int, float, complex.
-   String: Ordered, immutable.
-   List: Ordered, mutable.
-   Tuple: Ordered, immutable.
-   Set: Unordered, unique.
-   Dictionary: Key-value pairs.
-   Dictionary keys must be immutable.
