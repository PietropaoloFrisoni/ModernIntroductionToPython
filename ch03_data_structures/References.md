# Chapter 3 — References
### Modern Introduction to Python from scratch

---

## Reference 1: [Built-in Types (complete overview)](https://docs.python.org/3/library/stdtypes.html)
**The comprehensive official reference for all Python built-in types, including numeric types, sequences, mappings, sets, and more. The single most complete reference for the data structures covered in this chapter.**

This page is large and can be overwhelming. I'd use it as a reference when you need to look something up, not as reading material from top to bottom.

---

## Reference 2: [Text Sequence Type — `str`](https://docs.python.org/3/library/stdtypes.html#text-sequence-type-str)
**Official documentation for Python strings, including the complete table of string methods (`.upper()`, `.split()`, `.join()`, `.replace()`, `.strip()`, etc.), formatting, and encoding behaviour.**

The string method table is the part I refer to most often. When I can't remember the exact name of a method, this is where I look.

---

## Reference 3: [Sequence Types — `list`, `tuple`, `range`](https://docs.python.org/3/library/stdtypes.html#sequence-types-list-tuple-range)
**Official documentation for Python's sequence types. Covers all common and mutable-sequence-specific operations, including indexing, slicing, `append`, `extend`, `insert`, `remove`, `sort`, and `reverse`.**

Note the difference between the table of operations available to all sequences and the table of operations available only to mutable sequences.

---

## Reference 4: [Mapping Types — `dict`](https://docs.python.org/3/library/stdtypes.html#mapping-types-dict)
**Official documentation for Python dictionaries, including all dict methods (`.keys()`, `.values()`, `.items()`, `.get()`, `.update()`, `.pop()`), dict comprehensions, and the guarantee of insertion-order preservation from Python 3.7 onwards.**

Dictionaries are one of Python's greatest strengths (as mentioned in the video, they are essentially hash tables). The insertion-order guarantee is something that catches people off guard if they're used to older Python versions.

---

## Reference 5: [Set Types — `set`, `frozenset`](https://docs.python.org/3/library/stdtypes.html#set-types-set-frozenset)
**Official documentation for Python sets and frozen sets, including set operations (union, intersection, difference, symmetric difference), subset and superset tests, and the `frozenset` immutable variant.**

Sets are often underused by beginners. They are the right tool whenever you need uniqueness or fast membership testing.

---

## Reference 6: [Data Structures — Tutorial](https://docs.python.org/3/tutorial/datastructures.html)
**Official Python tutorial chapter on data structures. Provides practical coverage of lists as stacks and queues, list comprehensions, nested list comprehensions, tuples, sets, and dictionaries. The most readable introduction to these topics in the official documentation.**

Probably the most readable of all the references in this chapter.

---

## Reference 7: [The `collections` Module](https://docs.python.org/3/library/collections.html)
**Official documentation for the `collections` module, which provides specialised container types beyond the built-ins. Covers `deque`, `Counter`, `defaultdict`, `OrderedDict`, and `namedtuple`.**

Don't feel obliged to read this all at once (just know the module exists and come back when you need a `Counter` or a `defaultdict`).

---

## Reference 8: [`collections.deque`](https://docs.python.org/3/library/collections.html#collections.deque)
**Official documentation for `deque` (double-ended queue), which supports O(1) appends and pops from both ends. Explains when to prefer it over a list and documents its full API including `appendleft`, `popleft`, and `rotate`.**

I leave this here because we used `deque` in the notebook. Useful to know when lists are not the right choice.
