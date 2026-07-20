# Python Chapter 8A -- Slicing

> **Filename:** `Python_Chapter_8A_Slicing.md`

## What is Slicing?

Slicing extracts a portion of a sequence without modifying the original
object (unless using slice assignment on mutable sequences).

**General Syntax**

``` python
sequence[start:stop:step]
```

-   `start` -- starting index (inclusive)
-   `stop` -- ending index (exclusive)
-   `step` -- increment/decrement

------------------------------------------------------------------------

## Indexing vs Slicing

  Feature      Indexing         Slicing
  ------------ ---------------- --------------
  Returns      Single element   New sequence
  Syntax       `a[3]`           `a[1:5]`
  Copy         No               Usually Yes
  Complexity   O(1)             O(k)

------------------------------------------------------------------------

## Default Values

``` python
a[:]
a[:5]
a[5:]
a[::2]
a[::-1]
```

Defaults:

-   `start = 0`
-   `stop = len(sequence)`
-   `step = 1`

------------------------------------------------------------------------

## Positive Examples

``` python
text = "MachineLearning"

text[0:7]
text[7:]
text[:7]
text[::2]
text[1::2]
```

------------------------------------------------------------------------

## Negative Indexing

``` python
text[-1]
text[-5:]
text[:-3]
text[-8:-2]
```

------------------------------------------------------------------------

## Negative Step

``` python
text[::-1]
text[::-2]
text[10:2:-1]
```

------------------------------------------------------------------------

# Slicing Across Python Data Types

## Strings

``` python
name = "Python"

name[:3]
name[::-1]
```

------------------------------------------------------------------------

## Lists

``` python
nums = [10,20,30,40,50]

nums[1:4]
nums[::-1]
nums[::2]
```

### Slice Assignment

``` python
nums[1:3] = [100,200]
```

### Delete Slice

``` python
del nums[2:5]
```

------------------------------------------------------------------------

## Tuples

``` python
t = (1,2,3,4,5)

t[1:4]
t[::-1]
```

Immutable---slicing creates a new tuple.

------------------------------------------------------------------------

## Range

``` python
r = range(20)

r[5:10]
r[::-1]
```

------------------------------------------------------------------------

## Bytes

``` python
b = b"abcdef"

b[2:5]
```

------------------------------------------------------------------------

## Bytearray

``` python
data = bytearray(b"abcdef")

data[1:4]
```

------------------------------------------------------------------------

## array.array

``` python
from array import array

arr = array("i",[1,2,3,4,5])

arr[1:4]
```

------------------------------------------------------------------------

## memoryview

``` python
data = memoryview(bytes([1,2,3,4,5]))

data[1:4]
```

Useful for avoiding unnecessary copies.

------------------------------------------------------------------------

# slice() Object

``` python
s = slice(1,8,2)

text[s]
```

Equivalent to:

``` python
text[1:8:2]
```

------------------------------------------------------------------------

# Custom Objects

Objects can support slicing by implementing:

``` python
__getitem__()
```

Python passes a `slice` object automatically.

------------------------------------------------------------------------

# Copying with Slicing

``` python
copy = lst[:]
```

Creates a **shallow copy**.

------------------------------------------------------------------------

# Common Patterns

``` python
a[::-1]      # Reverse

a[::2]       # Every second element

a[-3:]       # Last 3

a[:-1]       # Everything except last

a[:]         # Copy

a[1:-1]      # Middle

a[::3]       # Every third
```

------------------------------------------------------------------------

# Performance

  Operation   Complexity
  ----------- ------------
  Indexing    O(1)
  Slicing     O(k)

where **k = number of copied elements**.

------------------------------------------------------------------------

# Common Mistakes

``` python
a[::0]
```

Raises

``` text
ValueError: slice step cannot be zero
```

Remember:

-   stop index is excluded
-   negative step reverses direction
-   slicing returns a new object for built-in immutable sequences

------------------------------------------------------------------------

# Best Practices

-   Prefer readable slices.
-   Avoid magic numbers.
-   Use `slice()` when reusing the same slice repeatedly.
-   Use slicing instead of loops for simple extraction.
-   Remember that list slicing is a shallow copy.

------------------------------------------------------------------------

# Interview Questions

1.  Why is slicing O(k)?
2.  Does slicing create a copy?
3.  Why is the stop index excluded?
4.  What does `[::-1]` do?
5.  Difference between indexing and slicing?
6.  What is a `slice` object?
7.  How does slice assignment work?
8.  Why does `a[::2] = values` require matching lengths?

------------------------------------------------------------------------

# Cheat Sheet

``` python
a[:]
a[1:]
a[:-1]
a[-3:]
a[::2]
a[1::2]
a[::-1]
a[::-2]
a[-5:-1]
a[2:10:3]
```
