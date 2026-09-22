# Equality-only grouping lower bound

↑ **Parent:** [Equality test](equality-test.md)

In the comparison model exposing only an [equality test](equality-test.md) between otherwise opaque values, partitioning $n$ values into [equivalence classes](equivalence-class.md) takes $\Omega(n^2)$ tests in the worst case. Run the algorithm on pairwise distinct values. If any pair remains untested, changing just those two values to equal is consistent with every answer observed so far but changes the required output partition. Every pair must therefore be tested. With a compatible [total order](total-order.md), [comparison sort](comparison-sort.md) can instead group equal values in $O(n\log n)$ time.

## ↑ Ancestors (4)

1. [Equality test](equality-test.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/3/f/solution.md)
