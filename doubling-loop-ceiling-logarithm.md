# Doubling-loop ceiling logarithm

↑ **Parent:** [Logarithm](logarithm.md)

For positive $x$, start at $i=0,y=1$ and repeatedly increment $i$ and double $y$ while $y<x$. In exact [integer arithmetic](integer-arithmetic.md), the [loop invariant](loop-invariant.md) $y=2^i$ together with $i=0$ or $2^{i-1}<x$ yields $i=\lceil\log_2x\rceil$ at exit. For fixed-width arithmetic, this proof requires every useful doubling to be representable. A signed 32-bit doubling variable becomes negative at $2^{31}$ and then zero, so the loop need not terminate for inputs above $2^{30}$. Widening the variable to a signed 64-bit type repairs the algorithm for positive 32-bit inputs.

## ↑ Ancestors (8)

1. [Logarithm](logarithm.md)
2. [Exponential function](exponential-function.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/2/c/solution.md)
