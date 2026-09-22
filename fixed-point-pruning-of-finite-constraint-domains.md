# Fixed-point pruning of finite constraint domains

↑ **Parent:** [Constraint propagation](constraint-propagation.md)

Repeatedly apply a [constraint propagation](constraint-propagation.md) operation that only deletes values from finite [constraint domains](constraint-domain.md), preserves their order, and preserves every valid assignment. The sum of domain sizes is a nonnegative [loop variant](loop-variant.md) at every changing step, so repetition reaches a [fixed point](fixed-point.md). For $N$ initial candidate values there are at most $N$ changing steps. An empty domain proves failure; a non-singleton fixed point may still require [backtracking](backtracking.md) or explicit enumeration. Preservation of solutions, rather than mere deletion, is essential.

## ↑ Ancestors (8)

1. [Constraint propagation](constraint-propagation.md)
2. [Constraint satisfaction problem](constraint-satisfaction-problem.md)
3. [Search problem](search-problem.md)
4. [Computational problem](computational-problem.md)
5. [Computational complexity theory](computational-complexity-theory.md)
6. [Theoretical computer science](theoretical-computer-science-split.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/3/e/solution.md)
