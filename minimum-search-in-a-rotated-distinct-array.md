# Minimum search in a rotated distinct array

↑ **Parent:** [Binary search](binary-search.md)

In a nonempty rotation of a strictly increasing [array](array-data-structure.md), keep an inclusive interval containing its minimum. Compare its midpoint with its right endpoint. If the midpoint is larger, the minimum lies strictly to the right of the midpoint; otherwise the midpoint-to-right segment is increasing and the minimum lies at or left of the midpoint. The interval at least halves until one index remains. The cyclic predecessor of this minimum holds the maximum, so both extrema are found with $O(\log n)$ comparisons. Distinctness makes the two-way comparison decisive.

## ↑ Ancestors (4)

1. [Binary search](binary-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/5/b/solution.md)
