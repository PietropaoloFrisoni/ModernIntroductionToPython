# Chapter 1 — References
### Introduction to Modern Python

---

## Reference 1: [Numeric Types: int, float, complex](https://docs.python.org/3/library/stdtypes.html#numeric-types-int-float-complex)
**Official Python documentation covering the three built-in numeric types introduced in this chapter: integers, floating-point numbers, and complex numbers. Includes the complete table of supported operations and type conversion rules.**

This is probably the page I used to have open most often when writing numerical code. The operation table halfway down is particularly useful.

---

## Reference 2: [Operator Precedence](https://docs.python.org/3/reference/expressions.html#operator-precedence)
**Official Python language reference table listing all operators in order of precedence, from lowest to highest. Essential reading for understanding how Python evaluates complex expressions involving arithmetic, comparison, and logical operators.**

Worth bookmarking (much easier to look this up than to memorize it).

---

## Reference 3: [Floating Point Arithmetic: Issues and Limitations](https://docs.python.org/3/tutorial/floatingpoint.html)
**Official Python tutorial section explaining why floating-point numbers cannot always be represented exactly in binary, and what consequences this has for arithmetic and rounding. Directly related to the precision section of this chapter.**

If you have time to read only one reference in this chapter, I think this one is the most appropriate. The floating-point precision issue genuinely surprises people the first time they encounter it, and this page explains it better than anywhere else.

---

## Reference 4: [The `math` Module](https://docs.python.org/3/library/math.html)
**Official documentation for the `math` module, which provides `math.nan`, `math.inf`, `math.isnan()`, `math.isinf()`, and a wide range of mathematical functions for real-valued computation.**

---

## Reference 5: [The `decimal` Module](https://docs.python.org/3/library/decimal.html)
**Official documentation for the `decimal` module, which provides a `Decimal` type for exact decimal arithmetic. The right tool when float precision issues matter — for example, in financial calculations.**

You probably won't need this in everyday code, but it's good to know it exists.

---

## Reference 6: [The `fractions` Module](https://docs.python.org/3/library/fractions.html)
**Official documentation for the `fractions` module, which provides the `Fraction` type for exact rational arithmetic. Covers construction, arithmetic operations, and conversion to and from other numeric types.**

Same as above: niche, but extremely useful in the right context.

---

## Reference 7: [The `sys` Module — `getsizeof`](https://docs.python.org/3/library/sys.html#sys.getsizeof)
**Official documentation for `sys.getsizeof()`, used in the memory footprint section of this chapter. Includes an important note clarifying that the result reflects the size of the Python object wrapper, not just the raw numeric data.**

---

## Reference 8: [Truth Value Testing](https://docs.python.org/3/library/stdtypes.html#truth-value-testing)
**Official documentation describing how Python evaluates objects in a boolean context. Explains which values are considered falsy (such as `0`, `0.0`, and `None`) — directly relevant to the types section of this chapter.**

Easy to overlook, but this is actually essential reading. Understanding what Python considers "truthy" shows up constantly in real code.

---

## Reference 9: [Constants — `None`](https://docs.python.org/3/library/constants.html#None)
**Official documentation for `None`, Python's built-in constant representing the absence of a value. Clarifies its type (`NoneType`), its uniqueness as a singleton, and why `is None` is the correct way to test for it.**

Short page, worth reading in full. Testing with `is None` instead of `== None` is one of those Python conventions that trips up beginners more often than it should.
