# Section 2 -- Theory Questions

# Topic 1: Python Basics

## 1. Explain how Python code executes internally.

**Answer:**

When a Python program runs, it goes through the following steps:

1.  Source Code (.py file)
2.  Compilation into Bytecode (.pyc)
3.  Bytecode is executed by the Python Virtual Machine (PVM)
4.  The PVM executes instructions line by line.
5.  Output is produced.

Flow:

``` text
Python Source Code (.py)
        ↓
Python Compiler
        ↓
Bytecode (.pyc)
        ↓
Python Virtual Machine (PVM)
        ↓
Program Output
```

## 2. What is the Python Interpreter?

The Python Interpreter is software that reads, compiles, and executes
Python code.

Functions: - Reads Python code - Converts it to bytecode - Executes
bytecode using the PVM - Displays output

Examples: - CPython - PyPy - Jython - IronPython

## 3. What is REPL?

REPL stands for Read, Evaluate, Print, Loop. It is Python's interactive
shell for executing code immediately.

## 4. What happens when Python executes a file?

1.  Reads the source code.
2.  Checks syntax.
3.  Compiles to bytecode.
4.  Stores bytecode in **pycache** (optional).
5.  PVM executes the bytecode.
6.  Displays output.

## 5. What is Bytecode?

Bytecode is platform-independent intermediate code generated from Python
source code and executed by the PVM.

## 6. What is PVM (Python Virtual Machine)?

The PVM executes Python bytecode, manages memory, handles function calls
and exceptions, and produces output.

## 7. Explain Compilation vs Interpretation.

  -----------------------------------------------------------------------
  Compilation                         Interpretation
  ----------------------------------- -----------------------------------
  Converts the whole program before   Executes code line by line.
  execution.                          

  Produces bytecode/machine code.     Executes through an interpreter.

  Faster after compilation.           Slower because execution is line by
                                      line.
  -----------------------------------------------------------------------

Python first compiles to bytecode and then interprets it using the PVM.

## 8. What is Duck Typing?

Duck Typing means Python focuses on an object's behavior rather than its
type.

> "If it walks like a duck and quacks like a duck, it is a duck."

Example:

``` python
class Dog:
    def speak(self):
        print("Bark")

class Cat:
    def speak(self):
        print("Meow")

def animal_sound(animal):
    animal.speak()

animal_sound(Dog())
animal_sound(Cat())
```

Output:

``` text
Bark
Meow
```

# Quick Revision

-   Python Interpreter: Executes Python code.
-   REPL: Read-Evaluate-Print-Loop.
-   Bytecode: Intermediate code.
-   PVM: Executes bytecode.
-   Compilation: Converts source code to bytecode.
-   Interpretation: Executes bytecode.
-   Duck Typing: Behavior matters more than type.
-   Execution Flow: .py → Bytecode → PVM → Output.
