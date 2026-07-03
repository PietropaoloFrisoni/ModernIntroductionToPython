# Chapter 10 — References
### Introduction to Modern Python

---

## Reference 1: [Errors and Exceptions — Tutorial](https://docs.python.org/3/tutorial/errors.html)
**Official Python tutorial chapter on exceptions. Covers syntax errors, raising exceptions, handling exceptions with `try`/`except`/`else`/`finally`, defining custom exception classes, and exception chaining. The most complete single introduction to the topics of this chapter.**

A good complement to the notebook (basically it covers everything in a slightly different order and with different examples).

---

## Reference 2: [Built-in Exceptions](https://docs.python.org/3/library/exceptions.html)
**Official documentation for all built-in exception and warning classes. Describes each exception's meaning, when it is raised by the interpreter, and what its attributes contain. The essential reference for knowing which exception type to catch or raise.**

I used this page constantly when I was trying to remember which exception to catch or raise for a given situation.

---

## Reference 3: [Exception Hierarchy](https://docs.python.org/3/library/exceptions.html#exception-hierarchy)
**Official diagram showing the full inheritance tree of all built-in exceptions, from `BaseException` at the root down through `Exception`, `ArithmeticError`, `LookupError`, and every leaf class. Understanding the hierarchy determines how `except` clauses catch exceptions.**

Worth spending a few minutes with this diagram. Knowing the hierarchy tells you exactly which `except` clauses will catch which exceptions.

---

## Reference 4: [The `raise` Statement](https://docs.python.org/3/reference/simple_stmts.html#the-raise-statement)
**Official language reference for the `raise` statement. Defines bare `raise` (re-raise), `raise ExceptionType`, `raise instance`, and the `raise NewException from original` exception-chaining form.**

Short page, worth reading in full. The `raise X from Y` form is particularly important to understand for writing clean, informative error messages.

---

## Reference 5: [The `try` Statement](https://docs.python.org/3/reference/compound_stmts.html#the-try-statement)
**The authoritative technical specification for the `try` compound statement, including the precise semantics of `except`, `else`, and `finally` clauses and their interactions with each other.**

Worth reading when you're unclear about the exact interaction between `else` and `finally`.

---

## Reference 6: [PEP 3134 — Exception Chaining and Embedded Tracebacks](https://peps.python.org/pep-3134/)
**The original proposal that introduced exception chaining (`raise X from Y`) into Python 3. Explains `__cause__` (explicit chaining) and `__context__` (implicit chaining), and why preserving the original traceback matters for debugging.**

Exception chaining is one of those features you only fully appreciate when you're debugging a complex failure (I had to do this more than once). Understanding `__cause__` vs `__context__` saves a lot of confusion.
