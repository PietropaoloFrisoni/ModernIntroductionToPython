# Chapter 6 — References
### Introduction to Modern Python

---

## Reference 1: [The `functools` Module](https://docs.python.org/3/library/functools.html)
**Official documentation for the `functools` module — the standard library home for decorator utilities. The single most important reference for this chapter, covering `wraps`, `cache`, `lru_cache`, `partial`, and `reduce`.**

---

## Reference 2: [`functools.wraps`](https://docs.python.org/3/library/functools.html#functools.wraps)
**Official documentation for `functools.wraps`, the decorator that copies `__name__`, `__doc__`, `__annotations__`, and other attributes from the wrapped function to the wrapper. Essential for writing decorators that behave transparently under introspection.**

I usually use `@wraps` when writing decorators (your future self will thank you when you try to debug something).

---

## Reference 3: [`functools.cache`](https://docs.python.org/3/library/functools.html#functools.cache)
**Official documentation for `functools.cache` (added in Python 3.9): an unbounded memoization decorator equivalent to `lru_cache(maxsize=None)`. Explains its semantics, thread-safety notes, and how to inspect or clear the cache.**

This is probably the most useful decorator in the standard library. If you have a pure function that gets called repeatedly with the same arguments, this is often the fastest optimisation you can make.

---

## Reference 4: [`functools.lru_cache`](https://docs.python.org/3/library/functools.html#functools.lru_cache)
**Official documentation for `functools.lru_cache`, a bounded memoization decorator that evicts least-recently-used entries when the cache reaches `maxsize`. Covers the `typed` parameter and the `cache_info()` and `cache_clear()` methods.**

The bounded version of `cache`. `cache_info()` is particularly handy for understanding cache hit rates.

---

## Reference 5: [Decorator Syntax — Function Definitions](https://docs.python.org/3/reference/compound_stmts.html#function-definitions)
**Official Python language reference section covering the `@decorator` syntax. Defines precisely what the decorator expression may contain (any callable expression) and how it is applied to the function object.**

---

## Reference 6: [PEP 318 — Decorators for Functions and Methods](https://peps.python.org/pep-0318/)
**The original proposal that introduced the `@decorator` syntax. Explains the motivation (replacing verbose `func = decorator(func)` assignments), the design decisions, and the alternatives that were considered.**

Interesting historically. The `@` syntax was actually controversial at the time. Worth reading once to understand why it was designed the way it was.
