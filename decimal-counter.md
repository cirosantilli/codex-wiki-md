# Decimal counter

↑ **Parent:** [Data structure](data-structure-split.md)

A [decimal counter](decimal-counter.md) stores a nonnegative [integer](integer-split.md) using an [array](array-data-structure.md) of base-ten [digits](numerical-digit.md), with the least significant [digit](numerical-digit.md) first. Increment resets trailing nines and increases the next [digit](numerical-digit.md), or wraps modulo $10^k$ if all $k$ [digits](numerical-digit.md) are nines. Starting at zero, the exact number of [digit](numerical-digit.md) changes in $n$ increments is $\sum_{i=0}^{k-1}\lfloor n/10^i\rfloor\leq10n/9$. This is an [aggregate analysis](aggregate-analysis.md) proving a constant [amortized cost](amortized-cost.md) per increment under unit-cost [digit](numerical-digit.md) updates. An arbitrary initial value contributes an additional $O(k)$ in [Big O notation](big-o-notation.md).

## ↑ Ancestors (3)

1. [Data structure](data-structure-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Decimal counter](decimal-counter.md)
- [Advanced data structures and algorithms](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/advanced-data-structures-and-algorithms-split.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/advanced-data-structures-and-algorithms/1/b/solution.md)
