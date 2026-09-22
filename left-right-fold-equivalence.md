# Left-right fold equivalence

↑ **Parent:** [List fold](list-fold.md)

For finite [lists](list-abstract-data-type.md), if $x\oplus(y\otimes z)=(x\oplus y)\otimes z$ and $x\oplus a=a\otimes x$, then the [right fold](list-fold.md) with step $\oplus$ and seed $a$ equals the [left fold](left-fold.md) with step $\otimes$ and seed $a$. The two steps need not be identical. Equality of the resulting values does not imply equal [time complexity](time-complexity.md); [list concatenation](list-concatenation.md) is an important example.

## ↑ Ancestors (5)

1. [List fold](list-fold.md)
2. [Functional programming](functional-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/2/b/solution.md)
