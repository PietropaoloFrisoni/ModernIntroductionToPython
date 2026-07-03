# Chapter 11 — References
### Introduction to Modern Python

---

## Reference 1: [Built-in Function — `open()`](https://docs.python.org/3/library/functions.html#open)
**Official documentation for `open()`, the gateway to file I/O. Documents every parameter: `file`, `mode`, `buffering`, `encoding`, `errors`, `newline`, and `closefd`. Explains the difference between text mode and binary mode and when each should be used.**

The parameter list for `open()` is longer than most people realise. Worth looking at the `encoding` and `errors` parameters in particular.

---

## Reference 2: [Reading and Writing Files — Tutorial](https://docs.python.org/3/tutorial/inputoutput.html#reading-and-writing-files)
**Official Python tutorial section on file I/O. Covers opening files with `with`, reading with `read()`, `readline()`, and `readlines()`, writing, and the `f.tell()` / `f.seek()` positioning methods.**

The most readable introduction (covers all the basics you'll use day to day).

---

## Reference 3: [The `io` Module](https://docs.python.org/3/library/io.html)
**Official documentation for the `io` module, which defines the abstract base classes behind all I/O in Python: `RawIOBase`, `BufferedIOBase`, and `TextIOBase`. Essential for understanding the layered I/O architecture and for writing custom file-like objects.**

More advanced. You typically don't need this unless you're writing custom file-like objects. Worth knowing it exists.

---

## Reference 4: [The `pathlib` Module](https://docs.python.org/3/library/pathlib.html)
**Official documentation for `pathlib`, the modern, object-oriented approach to filesystem paths. Covers `Path` construction, navigating directories, reading and writing files directly via `Path` objects, and cross-platform path handling.**

I strongly recommend switching to `pathlib` for any path handling. It's much cleaner than string concatenation or `os.path`.

---

## Reference 5: [The `contextlib` Module](https://docs.python.org/3/library/contextlib.html)
**Official documentation for the `contextlib` module. Covers `@contextmanager` (writing context managers with a generator function), `suppress`, `redirect_stdout`, `ExitStack`, and `asynccontextmanager`.**

Beyond `@contextmanager`, `contextlib.suppress` is a genuinely useful tool that I used to reach for regularly.

---

## Reference 6: [The `with` Statement](https://docs.python.org/3/reference/compound_stmts.html#the-with-statement)
**The authoritative language reference for the `with` statement. Defines the context manager protocol precisely: when `__enter__` and `__exit__` are called, how the exception information is passed to `__exit__`, and what it means for `__exit__` to return a truthy value.**

Worth reading if you are ever confused about what happens to an exception raised inside a `with` block.

---

## Reference 7: [Data Model — Context Managers](https://docs.python.org/3/reference/datamodel.html#context-managers)
**Official language reference defining the context manager protocol (`__enter__` and `__exit__`). Specifies the exact signatures and return value semantics, making this the definitive reference for implementing custom context manager classes.**

If you want to write a context manager as a class rather than using `@contextmanager`, this is where to look for the exact signatures.
