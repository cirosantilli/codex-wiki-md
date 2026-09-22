# Lower-bound binary search invariant

↑ **Parent:** [Binary search](binary-search.md)

In a nondecreasing [array](array-data-structure.md), the first position whose entry is at least $x$ is found by maintaining a half-open unresolved interval $[l,h)$. Entries before $l$ are smaller than $x$; entries from $h$ onward are at least $x$. Initially $l=c_0,h=c_1$. At midpoint $m$, replace $l$ by $m+1$ if $A[m]<x$, and otherwise replace $h$ by $m$. [Monotonicity](monotonic-function.md) preserves the [loop invariant](loop-invariant.md), and $h-l$ decreases. On exit $l=h$ is the first qualifying position, or $c_1$ if no such entry exists. Repeated values and endpoint cuts require no additional case.

## ↑ Ancestors (4)

1. [Binary search](binary-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/2/f/solution.md)
