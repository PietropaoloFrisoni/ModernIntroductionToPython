# Intermezzo 2 — References
### Modern Introduction to Python from scratch

---

## Reference 1: [Data Model — Objects, Values, and Types](https://docs.python.org/3/reference/datamodel.html#objects-values-and-types)
**Official Python language reference section defining what an object is in Python: every object has an identity, a type, and a value. Explains the distinction between mutable and immutable objects at the language specification level.**

In my opinion, the most important single reference for understanding this entire intermezzo. Everything follows from the definition of an object as something with identity, type, and value.

---

## Reference 2: [Built-in Functions (complete index)](https://docs.python.org/3/library/functions.html)
**The complete official index of all Python built-in functions, including `id()`, `type()`, `isinstance()`, `len()`, and `repr()`. One of the most frequently consulted references in everyday Python programming.**

---

## Reference 3: [Comparisons — `is` and `is not`](https://docs.python.org/3/reference/expressions.html#is)
**Official Python language reference for the identity operators `is` and `is not`. Defines precisely what they test, how they relate to `id()`, and when they should be used instead of `==`.**

Short section, but crucial. The warning about `is` being unreliable for integers and strings due to interning is the kind of thing that causes hard-to-reproduce bugs. We will talk about interning in a more advanced course.

---

## Reference 4: [Augmented Assignment Statements](https://docs.python.org/3/reference/simple_stmts.html#augmented-assignment-statements)
**Official language reference for augmented assignment operators (`+=`, `-=`, `*=`, etc.). Explains how they are evaluated and, crucially, how their behaviour differs between mutable and immutable types — the key insight from this intermezzo.**

This formalises exactly what we demonstrated in the notebook with lists vs integers.

---

## Reference 5: [Built-in Function — `id()`](https://docs.python.org/3/library/functions.html#id)
**Official documentation for `id()`, which returns the identity of an object — an integer that is unique and constant for the object's lifetime. In CPython this is the memory address, though the specification does not guarantee this.**

Worth noting the distinction between what CPython happens to do (memory address) and what the specification actually guarantees (unique integer). They're not the same thing.

---

## Reference 6: [Built-in Function — `isinstance()`](https://docs.python.org/3/library/functions.html#isinstance)
**Official documentation for `isinstance()`, the correct way to test whether an object is an instance of a class or a tuple of classes. Covers its interaction with inheritance and why it should be preferred over direct `type()` comparisons.**
