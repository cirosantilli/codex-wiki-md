# Distinct-index two-sum by suffix lower bounds

↑ **Parent:** [Binary search](binary-search.md)

For each candidate first index $i$ in a [sorted array](sorted-array.md), use [lower-bound search](lower-bound-search.md) for $t-a(i)$ only in the suffix starting at $i+1$. A matching result is automatically at a different position. The outer [loop invariant](loop-invariant.md) excludes all solutions whose smaller index precedes $i$; an unsuccessful suffix search extends this exclusion by one. Exhaustion proves absence of any pair. Searching all suffixes gives $O(N\log(N+1))$ [running time](running-time.md) and constant [auxiliary space](auxiliary-space.md). Compute the complement in a sufficiently wide type to avoid [integer overflow](integer-overflow.md) before comparison.

## ↑ Ancestors (4)

1. [Binary search](binary-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/1/e/solution.md)
- [Two-sum problem](two-sum-problem.md)
