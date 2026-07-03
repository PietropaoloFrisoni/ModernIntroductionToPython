# Chapter 4 — References
### Introduction to Modern Python

---

## Reference 1: [Defining Functions — Tutorial](https://docs.python.org/3/tutorial/controlflow.html#defining-functions)
**Official Python tutorial section on defining functions. Covers `def`, return values, default arguments, keyword arguments, `*args`, `**kwargs`, and arbitrary argument lists — the complete practical introduction to functions in Python.**

Very readable. A good complement to the notebook, and it goes a bit further on some topics.

---

## Reference 2: [Function Definitions — Language Reference](https://docs.python.org/3/reference/compound_stmts.html#function-definitions)
**The authoritative technical specification for function definitions in Python. Covers parameter types in precise detail: positional-or-keyword, positional-only, keyword-only, `*args`, and `**kwargs`.**

More technical than the tutorial. Worth skimming the parameter types section.

---

## Reference 3: [Built-in Functions (complete index)](https://docs.python.org/3/library/functions.html)
**The complete official index of all Python built-in functions. Essential reference for understanding which capabilities are available without any imports.**

Every time you wonder "does Python have a built-in for this?", you can start here (I bookmarked this in my research bar).

---

## Reference 4: [PEP 257 — Docstring Conventions](https://peps.python.org/pep-0257/)
**The official style guide for Python docstrings. Defines the conventions for one-line and multi-line docstrings, how the `__doc__` attribute is populated, and how `help()` uses docstrings.**

Writing good docstrings is a real professional skill. This page is short and worth reading in full.

---

## Reference 5: [The `typing` Module](https://docs.python.org/3/library/typing.html)
**Official documentation for the `typing` module, which provides the building blocks for type hints: `Optional`, `Union`, `List`, `Dict`, `Tuple`, `Callable`, and more. The reference for everything related to type annotation in Python.**

Note: for modern Python (3.9+), you can often skip this module entirely and use built-in types directly for annotations — `list[int]` instead of `typing.List[int]`, for example. The `typing` module is still needed for some advanced cases, but a lot of stuff has been deprecated.

---

## Reference 6: [PEP 484 — Type Hints](https://peps.python.org/pep-0484/)
**The original proposal that introduced type hints into Python. Explains the motivation, the design decisions, and how the type annotation system interacts with runtime behaviour — which is to say, not at all: hints are not enforced.**

Worth reading if you want to understand why type hints work the way they do, especially the crucial detail that they are purely optional and never enforced at runtime.
