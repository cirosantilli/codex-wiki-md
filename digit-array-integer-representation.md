# Digit-array integer representation

↑ **Parent:** [Arbitrary-precision arithmetic](arbitrary-precision-arithmetic.md)

Store an [integer](integer-split.md) in a nonempty [array](array-data-structure.md) of [numeral digits](numerical-digit.md), with the least significant digit first and a fixed [radix](radix.md) $b\geq2$. Normalized digits satisfy $0\leq a_i<b$. High-order zeros do not change the value. Adding digit arrays coefficientwise or multiplying them by [discrete convolution](discrete-convolution.md) gives the correct value before normalization, because these operations add or multiply the corresponding powers of the radix. Exact temporary arithmetic, or a radix and accumulator size chosen to prevent [integer overflow](integer-overflow.md), is required.

**Table of contents**

- [Power-of-ten digit-block formatting](power-of-ten-digit-block-formatting.md)
- [Carry normalization of a digit array](carry-normalization-of-a-digit-array.md)

## ↑ Ancestors (6)

1. [Arbitrary-precision arithmetic](arbitrary-precision-arithmetic.md)
2. [Integer arithmetic](integer-arithmetic.md)
3. [Arithmetic](arithmetic-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Carry normalization of a digit array](carry-normalization-of-a-digit-array.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/1/e/solution.md)
