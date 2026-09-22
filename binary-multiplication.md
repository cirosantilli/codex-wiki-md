# Binary multiplication

↑ **Parent:** [Multiplication](multiplication.md)

For nonnegative integers with [binary representation](binary-number.md) $Y=\sum_{i=0}^{w-1}y_i2^i$, multiply by $X$ by summing the shifted terms $y_i2^iX$. Each term is either zero or a [left bit shift](left-bit-shift.md) of $X$. An unsigned $w$-[bit](bit.md) input pair needs at most $2w$ product [bits](bit.md), because $(2^w-1)^2<2^{2w}$. This expansion follows from distributivity and motivates a [binary multiplier](binary-multiplier.md).

## ↑ Ancestors (5)

1. [Multiplication](multiplication.md)
2. [Arithmetic](arithmetic-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Binary multiplier](binary-multiplier.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/digital-systems-linear-algebra-introduction-to-formal-proof/2/a/solution.md)
