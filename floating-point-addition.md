# Floating-point addition

↑ **Parent:** [Floating-point arithmetic](floating-point-arithmetic-split.md)

To add two finite [floating-point numbers](floating-point-number.md), compare their [exponents](exponent.md), shift the smaller [significand](significand.md) to a common [exponent](exponent.md), add or subtract the signed [significands](significand.md), normalize the result, and apply [floating-point rounding](floating-point-rounding.md). Extra low-order [bits](bit.md) are needed to determine correct rounding when shifting or cancellation discards information. A carry beyond the leading digit increases the [exponent](exponent.md); cancellation can decrease it. Unlike exact real [addition](addition.md), this operation need not be associative. Changing the child evaluation order in a fixed [binary expression tree](binary-expression-tree.md) need not change its parenthesization, whereas reassociation changes which intermediate results undergo [floating-point rounding](floating-point-rounding.md).

## ↑ Ancestors (6)

1. [Floating-point arithmetic](floating-point-arithmetic-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/digital-systems-linear-algebra-introduction-to-formal-proof/6/d/solution.md)
