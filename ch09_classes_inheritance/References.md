# Chapter 9 — References
### Modern Introduction to Python from scratch

---

## Reference 1: [Classes — Tutorial (Inheritance and Multiple Inheritance)](https://docs.python.org/3/tutorial/classes.html#multiple-inheritance)
**Official Python tutorial section on multiple inheritance and the Method Resolution Order. Provides an accessible introduction to how Python resolves method lookups across a complex class hierarchy.**

The MRO section is the most important part. Python's approach to multiple inheritance is one of its more sophisticated design decisions.

---

## Reference 2: [Built-in Function — `super()`](https://docs.python.org/3/library/functions.html#super)
**Official documentation for `super()`. Explains how it returns a proxy object that delegates method calls to the next class in the MRO, why this is essential for cooperative multiple inheritance, and the difference between `super()` in Python 2 and Python 3.**

`super()` is one of those things that looks simple but has subtle depth. In the video, we only saw it in the simplest form. This is worth reading carefully.

---

## Reference 3: [Data Model — Customizing Class Creation](https://docs.python.org/3/reference/datamodel.html#customizing-class-creation)
**Official language reference section covering metaclasses, the MRO computation algorithm, and how class objects are created. Provides the formal specification behind the C3 linearization algorithm that Python uses to determine method resolution order.**

Advanced, and metaclasses are in here. You can have a very long Python career without ever needing to write one, but it's useful to know they exist and what problem they solve.

---

## Reference 4: [The `abc` Module — Abstract Base Classes](https://docs.python.org/3/library/abc.html)
**Official documentation for the `abc` module. Covers `ABC`, `ABCMeta`, `@abstractmethod`, `@abstractclassmethod`, and `@abstractstaticmethod`. Explains how abstract classes prevent instantiation until all abstract methods are implemented.**

I use `@abstractmethod` regularly in larger codebases. It's a simple but very effective way to enforce structure in a class hierarchy.

---

## Reference 5: [The `collections.abc` Module](https://docs.python.org/3/library/collections.abc.html)
**Official documentation for abstract base classes for containers. Defines the abstract interfaces for `Iterable`, `Iterator`, `Sequence`, `Mapping`, `Set`, and many more. Essential reading for understanding how duck typing and abstract classes work together in the standard library.**

This is where Python's own abstract interfaces live. It's the source of truth for what it means for an object to be an `Iterable`, a `Sequence`, or a `Mapping`.

---

## Reference 6: [PEP 3119 — Introducing Abstract Base Classes](https://peps.python.org/pep-3119/)
**The original proposal that introduced abstract base classes into Python. Explains the motivation (formalising the duck typing model), the role of `ABCMeta`, and the concept of virtual subclasses registered with `register()`.**

Worth reading if you want to understand the design philosophy behind ABCs — especially the concept of virtual subclasses.
