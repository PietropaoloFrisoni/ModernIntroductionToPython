# Intermezzo 1 — References
### Introduction to Modern Python

---

## Reference 1: [Truth Value Testing](https://docs.python.org/3/library/stdtypes.html#truth-value-testing)
**Official Python documentation describing how any object can be tested for truth. Lists every falsy value in the language — `None`, `False`, zero in all numeric types, and all empty containers — and explains how this integrates with `if` statements and boolean operators.**

This page is deceptively short but surprisingly important. I still refer back to it occasionally to double-check a specific edge case.

---

## Reference 2: [Boolean Type — `bool`](https://docs.python.org/3/library/stdtypes.html#boolean-type-bool)
**Official documentation for the `bool` type, including its relationship to `int` (as a subclass), and the exact definitions of `True` and `False`. Explains why `True + True == 2` is valid Python.**

The bool-as-int relationship is one of those things that surprises almost everyone the first time. Worth reading in full.

---

## Reference 3: [Boolean Operations — `and`, `or`, `not`](https://docs.python.org/3/library/stdtypes.html#boolean-operations-and-or-not)
**Official documentation for Python's three boolean operators, including their precedence relative to each other and the short-circuit evaluation rules for `and` and `or`. Explains that `and` and `or` return one of their operands rather than always returning `True` or `False`.**

The key insight here is that `and` and `or` return one of their operands, not necessarily a boolean. Unlocks a lot of idiomatic Python once you understand it.

---

## Reference 4: [Built-in Function — `any()`](https://docs.python.org/3/library/functions.html#any)
**Official documentation for `any()`, which returns `True` if at least one element of an iterable is truthy. Includes the precise specification of its behaviour on empty iterables.**

The empty iterable behaviour (`any([])` is `False`) is worth remembering.

---

## Reference 5: [Built-in Function — `all()`](https://docs.python.org/3/library/functions.html#all)
**Official documentation for `all()`, which returns `True` only if every element of an iterable is truthy. Includes the vacuous truth specification: `all([])` returns `True`.**

Same as above: `all([])` is `True` (vacuous truth). We discussed this in the intermezzo (this page is the formal specification).

---

## Reference 6: [Comparisons](https://docs.python.org/3/library/stdtypes.html#comparisons)
**Official documentation for all Python comparison operators (`==`, `!=`, `<`, `>`, `<=`, `>=`, `is`, `is not`, `in`, `not in`). Covers chaining, the distinction between value equality and identity, and operator precedence.**

The chaining behaviour (`1 < x < 10` is valid Python and works exactly as you'd hope) is one of my favourite language features.
