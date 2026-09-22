# Lower weighted median

↑ **Parent:** [Weighted median](weighted-median.md)

For ordered distinct values with positive weights summing to one, choose the first value whose cumulative weight reaches one half. The preceding cumulative weight is strictly below one half, and the remaining mass is at most one half, proving the displayed conditions. Stopping on equality chooses the lower value when a cumulative weight is exactly one half. Sorting followed by a scan takes $O(n\log n)$ time; [median of medians](median-of-medians.md) partitioning with a residual weight target gives deterministic [linear time](linear-time.md).

## ↑ Ancestors (8)

1. [Weighted median](weighted-median.md)
2. [Median](median.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/5/d/i/solution.md)
- [Weighted median](weighted-median.md)
