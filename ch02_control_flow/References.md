# Chapter 2 — References
### Modern Introduction to Python from scratch

---

## Reference 1: [More Control Flow Tools](https://docs.python.org/3/tutorial/controlflow.html)
**Official Python tutorial chapter dedicated to control flow. Covers `if`/`elif`/`else`, `for` loops, `range`, `break`, `continue`, `pass`, and function definitions. The most complete single reference for the topics of this chapter.**

This tutorial chapter is very readable. If you feel it, you can go through it even after finishing Chapter 2, since it reinforces everything with slightly different examples.

---

## Reference 2: [Compound Statements](https://docs.python.org/3/reference/compound_stmts.html)
**Official Python language reference for compound statements, including the precise grammar and semantics of `if`, `while`, `for`, `try`, and `with`. The authoritative technical specification behind the control flow constructs introduced in this chapter.**

Much more technical than the tutorial (don't be put off by the formal grammar notation). If you're curious about a specific statement, just search for it on the page.

---

## Reference 3: [The `range` Type](https://docs.python.org/3/library/stdtypes.html#range)
**Official documentation for the built-in `range` type. Explains that `range` is a lazy sequence, not a list, and covers its start, stop, step parameters and membership testing behaviour.**

Worth a careful read. `range` is lazier and more powerful than most beginners realise.

---

## Reference 4: [Built-in Function — `enumerate()`](https://docs.python.org/3/library/functions.html#enumerate)
**Official documentation for `enumerate()`, the idiomatic way to loop over an iterable when both the index and the value are needed. Covers the optional `start` parameter.**

One of those functions I use in almost every Python script.

---

## Reference 5: [Built-in Function — `zip()`](https://docs.python.org/3/library/functions.html#zip)
**Official documentation for `zip()`, which aggregates elements from multiple iterables into tuples. Explains its lazy evaluation in Python 3 and its behaviour when iterables have different lengths.**

Same as `enumerate`, once you start using `zip`, you won't go back to index-based loops for parallel iteration.

