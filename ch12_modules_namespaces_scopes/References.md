# Chapter 12 — References
### Modern Introduction to Python from scratch

---

## Reference 1: [Modules — Tutorial](https://docs.python.org/3/tutorial/modules.html)
**Official Python tutorial chapter on modules and packages. Covers importing, the module search path, compiling to bytecode, the standard module library, packages, and relative imports. The most accessible single reference for the topics of this chapter.**

Readable and complete. Worth going through alongside the notebook.

---

## Reference 2: [The Import System — Language Reference](https://docs.python.org/3/reference/import.html)
**The authoritative technical specification for Python's import system. Covers the entire import machinery: finders, loaders, the module spec, `sys.path`, `sys.modules`, namespace packages, and `importlib`. Essential for deep understanding of how `import` works under the hood.**

Advanced and very detailed. You don't need all of this for everyday Python, but if you've ever wondered exactly how `import` works under the hood, it's all here.

---

## Reference 3: [Naming and Binding](https://docs.python.org/3/reference/executionmodel.html#naming-and-binding)
**Official Python execution model section defining exactly how names are resolved at runtime. Provides the formal specification of the LEGB rule: local, enclosing, global, and built-in scopes.**

Worth reading once after finishing the chapter, to consolidate everything we covered about scopes into a single formal picture.

---

## Reference 4: [The `global` Statement](https://docs.python.org/3/reference/simple_stmts.html#the-global-statement)
**Official language reference for the `global` statement. Explains what it does (declares that a name in the current scope refers to the module-level global scope) and when it is and is not needed.**

Short page. The main practical takeaway: avoid `global` when you can (it makes code harder to reason about). There is almost always a cleaner alternative.

---

## Reference 5: [The `nonlocal` Statement](https://docs.python.org/3/reference/simple_stmts.html#the-nonlocal-statement)
**Official language reference for the `nonlocal` statement, which binds a name to a variable in the nearest enclosing scope that is not global. The formal specification behind the closure mutation pattern.**

Also short. `nonlocal` is the right tool inside closures when you need to mutate an enclosing variable, but like `global`, use it sparingly.

---

## Reference 6: [The `importlib` Module](https://docs.python.org/3/library/importlib.html)
**Official documentation for `importlib`, which provides programmatic access to Python's import machinery. Useful for dynamic imports, reloading modules, and understanding how the import system works at a deeper level.**

Advanced stuff. Most Python programmers never need to use `importlib` directly. Included for the curious.

---

## Reference 7: [`sys.path`](https://docs.python.org/3/library/sys.html#sys.path)
**Official documentation for `sys.path`, the list of directories that Python searches when looking for modules to import. Explains the order of precedence and how to modify it to make custom modules importable from any location.**

If you have ever had a module that Python couldn't find, `sys.path` is where the answer lives.
