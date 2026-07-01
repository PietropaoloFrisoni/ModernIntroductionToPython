# Chapter 7 — References
### Modern Introduction to Python from scratch

---

## Reference 1: [Classes — Tutorial](https://docs.python.org/3/tutorial/classes.html)
**Official Python tutorial chapter on classes. Covers scopes and namespaces, class and instance objects, method objects, class and instance variables, inheritance, and multiple inheritance. The most complete single reference for object-oriented programming in Python.**

This is genuinely one of the best parts of the official Python tutorial.

---

## Reference 2: [Class Definitions — Language Reference](https://docs.python.org/3/reference/compound_stmts.html#class-definitions)
**The authoritative technical specification for class definitions. Covers the class body execution model, how the class object is created, the role of the metaclass, and how the namespace is constructed.**

Much more technical than the video. Don't worry if the metaclass section is confusing (it is not needed for most Python programming).

---

## Reference 3: [Data Model — Objects, Values, and Types](https://docs.python.org/3/reference/datamodel.html#objects-values-and-types)
**Official Python language reference section defining what an object is. Every class instance is an object with an identity, a type, and a value. This section provides the formal underpinning of the class system.**

A bit abstract, but understanding that every Python entity is an object with identity, type, and value is the foundation of Python itself.

---

## Reference 4: [Built-in Function — `object`](https://docs.python.org/3/library/functions.html#object)
**Official documentation for `object`, the implicit base class of all Python classes. Documents the small set of methods every Python object inherits, including `__class__`, `__dir__`, and `__repr__`.**

---

## Reference 5: [Built-in Function — `type()`](https://docs.python.org/3/library/functions.html#type)
**Official documentation for `type()`. In its single-argument form it returns the type of any object, which is essential for introspecting class instances. In its three-argument form it dynamically creates new class objects.**

Note the two very different purposes depending on how many arguments you pass. The three-argument form (dynamic class creation) is advanced and you are unlikely to need it for a while.

---

## Reference 6: [Built-in Function — `isinstance()`](https://docs.python.org/3/library/functions.html#isinstance)
**Official documentation for `isinstance()`, the correct way to test whether an object is an instance of a given class or tuple of classes. Explains how it respects inheritance and why it should be preferred over direct `type()` comparisons.**

As mentioned in the video, prefer `isinstance()` over `type() ==` checks as it handles inheritance correctly and is the idiomatic way to test types in Python.
