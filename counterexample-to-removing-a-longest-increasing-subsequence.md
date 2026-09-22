# Counterexample to removing a longest increasing subsequence

↑ **Parent:** [Greedy algorithm](greedy-algorithm.md)

Repeatedly removing a longest [strictly increasing subsequence](strictly-increasing-subsequence.md) need not minimise the number of increasing subsequences in a partition. In $(2,4,1,3)$, removing $(2,3)$ leaves the decreasing pair $(4,1)$, for three subsequences overall. The partition $(2,4)$ and $(1,3)$ uses only two and is optimal because the original sequence is not increasing.

## ↑ Ancestors (4)

1. [Greedy algorithm](greedy-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/7/c/solution.md)
