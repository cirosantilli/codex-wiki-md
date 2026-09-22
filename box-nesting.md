# Box nesting

↑ **Parent:** [Dynamic programming](dynamic-programming.md)

Represent a $d$-dimensional box by its side-length vector and allow axis permutations. A box fits another when its permuted dimensions are all strictly smaller. Sorting each vector reduces containment to coordinatewise strict comparison, by the [sorted-coordinate criterion for box containment](sorted-coordinate-criterion-for-box-containment.md). For an input-order-preserving [subsequence](subsequence.md), the longest chain ending at position $j$ has one plus the greatest chain length at an earlier fitting position. This last-box decomposition proves the [dynamic programming](dynamic-programming.md) recurrence. Sorting all dimensions and testing all ordered index pairs takes $O(nd\log d+n^2d)$ [running time](running-time.md). Arbitrary reordering is a different convention, handled by the containment [Directed acyclic graph](directed-acyclic-graph.md).

**Table of contents**

- [Sorted-coordinate criterion for box containment](sorted-coordinate-criterion-for-box-containment.md)

## ↑ Ancestors (5)

1. [Dynamic programming](dynamic-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/8/d/ii/solution.md)
