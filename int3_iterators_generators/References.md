# Intermezzo 3 — References
### Modern Introduction to Python from scratch

---

## Reference 1: [Glossary — Iterator](https://docs.python.org/3/glossary.html#term-iterator)
**Official Python glossary definition of an iterator: an object implementing both `__iter__` and `__next__`. Explains the distinction between an iterator and an iterable, and describes the `StopIteration` protocol.**

The glossary definitions are surprisingly precise and worth reading verbatim. "Iterator" and "iterable" are two different things that beginners often confuse — reading both Reference 1 and Reference 2 together clarifies the distinction.

---

## Reference 2: [Glossary — Iterable](https://docs.python.org/3/glossary.html#term-iterable)
**Official Python glossary definition of an iterable: any object that can return an iterator from its `__iter__` method, or that defines `__getitem__` with integer indices. Explains how `for` loops and other language constructs use this protocol.**

---

## Reference 3: [Built-in Function — `iter()`](https://docs.python.org/3/library/functions.html#iter)
**Official documentation for `iter()`, which returns an iterator from an iterable. Covers both the single-argument form (calling `__iter__`) and the two-argument sentinel form.**

The two-argument sentinel form is worth knowing about, even if I don't use it often.

---

## Reference 4: [Built-in Function — `next()`](https://docs.python.org/3/library/functions.html#next)
**Official documentation for `next()`, which retrieves the next item from an iterator. Covers the optional default argument that prevents `StopIteration` from being raised when the iterator is exhausted.**

Short page. The default argument is a small but useful feature for consuming iterators without having to handle `StopIteration` manually.

---

## Reference 5: [Yield Expressions](https://docs.python.org/3/reference/expressions.html#yield-expressions)
**Official Python language reference for `yield` and `yield from`. The authoritative specification for generator functions, including how execution is suspended and resumed, how values are sent back in, and how `GeneratorExit` and `StopIteration` interact.**

More advanced, this covers `yield from` and the send protocol. Don't worry if parts of it are confusing. Most Python programmers use generators in their simplest form only.

---

## Reference 6: [Generator Expressions](https://docs.python.org/3/reference/expressions.html#generator-expressions)
**Official language reference for generator expressions — the concise lazy counterpart to list comprehensions. Defines the syntax, scoping rules, and evaluation order.**

Worth reading alongside Reference 5. Generator expressions and generator functions are closely related but have slightly different scoping rules.

---

## Reference 7: [PEP 255 — Simple Generators](https://peps.python.org/pep-0255/)
**The original proposal that introduced generator functions and the `yield` statement into Python. Explains the motivation, the design decisions, and the formal semantics — essential reading for understanding why generators work the way they do.**

Worth reading once to understand the original motivation behind generators. They were a significant design decision in Python's evolution.
