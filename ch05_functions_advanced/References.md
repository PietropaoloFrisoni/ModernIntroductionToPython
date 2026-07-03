# Chapter 5 — References
### Introduction to Modern Python

---

## Reference 1: [The `functools` Module](https://docs.python.org/3/library/functools.html)
**Official documentation for the `functools` module, which provides higher-order functions and tools for working with callables. Covers `partial`, `reduce`, `cache`, `lru_cache`, and `wraps` — all built on the first-class function model explored in this chapter.**

I use this module constantly in real work. `cache` alone is worth knowing about as it can basically make your code much, much faster almost for free and with no effort.

---

## Reference 2: [Built-in Function — `sorted()`](https://docs.python.org/3/library/functions.html#sorted)
**Official documentation for `sorted()`, which returns a new sorted list from any iterable. Covers the `key` and `reverse` parameters in detail, explaining how `key` functions are applied before comparisons.**

The `key` parameter is one of those things that unlocks a huge amount of power once you understand it.

---

## Reference 3: [Built-in Function — `map()`](https://docs.python.org/3/library/functions.html#map)
**Official documentation for `map()`, which applies a function to every item of an iterable and returns a lazy iterator. Explains its lazy evaluation in Python 3 and its multi-iterable form.**

In modern Python, list comprehensions are often clearer than `map`, but `map` has its place, especially in functional-style pipelines where you're composing several transformations.

---

## Reference 4: [Built-in Function — `filter()`](https://docs.python.org/3/library/functions.html#filter)
**Official documentation for `filter()`, which constructs a lazy iterator over elements of an iterable for which a function returns true. Explains the `None` shortcut that tests for truthiness directly.**

---

## Reference 5: [Lambda Expressions](https://docs.python.org/3/reference/expressions.html#lambda)
**Official Python language reference for `lambda` expressions. Defines precisely what a lambda can and cannot contain, and how it differs from a `def` function in terms of scope and usage.**

Short page. The key takeaway is that lambdas are limited by design (they can only contain a single expression). When in doubt, a named function is clearer.

---

## Reference 6: [Name Resolution](https://docs.python.org/3/reference/executionmodel.html#resolution-of-names)
**Official Python execution model section on how names are resolved at runtime. This is the formal specification behind closures: the rules that determine which variables an inner function captures from its enclosing scope.**

More advanced. It explains a few subtle behaviours that can surprise even experienced programmers.
