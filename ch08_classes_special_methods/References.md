# Chapter 8 — References
### Introduction to Modern Python

---

## Reference 1: [Data Model — Special Method Names (complete index)](https://docs.python.org/3/reference/datamodel.html#special-method-names)
**The definitive reference for all special methods in Python. Organises every dunder method by category: object creation, string representation, comparison, numeric emulation, container emulation, context managers, and more. The essential overview for this entire chapter.**

As mentioned in the video, there are way, way more dunder methods than we cover in the course. This page is the complete catalogue. Come back to it whenever you want to add new behaviour to a class.

---

## Reference 2: [Data Model — Basic Customization](https://docs.python.org/3/reference/datamodel.html#basic-customization)
**Official documentation covering the fundamental special methods: `__repr__`, `__str__`, `__bytes__`, `__format__`, `__hash__`, `__bool__`, and the six rich comparison methods (`__lt__`, `__le__`, `__eq__`, `__ne__`, `__gt__`, `__ge__`). Directly covers the most commonly implemented special methods.**

---

## Reference 3: [Data Model — Emulating Numeric Types](https://docs.python.org/3/reference/datamodel.html#emulating-numeric-types)
**Official documentation for the arithmetic special methods: `__add__`, `__sub__`, `__mul__`, `__truediv__`, `__floordiv__`, `__mod__`, `__pow__`, and their reflected and in-place variants. Explains the reflected method lookup protocol used when the left operand does not support the operation.**

The reflected method protocol (`__radd__`, `__rmul__`, etc.) is subtle. Worth reading carefully if you implement arithmetic on custom types.

---

## Reference 4: [Built-in Function — `property`](https://docs.python.org/3/library/functions.html#property)
**Official documentation for the `property` built-in, which turns a getter method into a descriptor. Covers how to add setters and deleters, and provides a complete example of the typical pattern using `@property`, `@name.setter`, and `@name.deleter`.**

One of my favourite Python features. Once you start using `@property`, you will find it hard to go back to raw attribute access in any code you care about.

---

## Reference 5: [Built-in Function — `classmethod`](https://docs.python.org/3/library/functions.html#classmethod)
**Official documentation for `classmethod`, which transforms a method so it receives the class (`cls`) rather than the instance as its first argument. Covers the use case of alternative constructors.**

Alternative constructors are the most common use case, as emphasized in the video. `datetime.fromisoformat()` is a well-known example in the standard library.

---

## Reference 6: [Built-in Function — `staticmethod`](https://docs.python.org/3/library/functions.html#staticmethod)
**Official documentation for `staticmethod`, which transforms a method so it receives neither the instance nor the class as an implicit argument. Explains when to use it and how it differs from a plain module-level function.**

Slightly controversial since many Python developers argue that a plain module-level function is usually clearer. But it has its place when the function is logically tied to the class and I have seen it quite often.

---

## Reference 7: [The `dataclasses` Module](https://docs.python.org/3/library/dataclasses.html)
**Official documentation for the `dataclasses` module, which automatically generates `__init__`, `__repr__`, `__eq__`, and optionally `__hash__` and ordering methods from class-level field annotations. Covers all decorator options, field metadata, post-init processing, and frozen dataclasses.**

If you find yourself writing `__init__`, `__repr__`, and `__eq__` repeatedly for simple data-holding classes, `@dataclass` is exactly what you need.
