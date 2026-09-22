# Natural-number fold

↑ **Parent:** [Structural recursion](structural-recursion.md)

For `data Natural = Zero | Succ Natural`, replace `Zero` by a base value and `Succ` by a step [function](function-split.md): `foldNat g a Zero = a` and `foldNat g a (Succ n) = g (foldNat g a n)`. On a finite total [natural number](natural-number.md) $n$ this iterates $g$ exactly $n$ times.

**Table of contents**

- [Natural-number fold fusion law](natural-number-fold-fusion-law.md)

## ↑ Ancestors (5)

1. [Structural recursion](structural-recursion.md)
2. [Functional programming](functional-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/1/f/solution.md)
