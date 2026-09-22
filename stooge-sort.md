# Stooge sort

↑ **Parent:** [Sorting algorithm](sorting-algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stooge_sort)

First exchange the endpoints of the current subarray if they are out of order. For current length $m>2$, put $k=\lfloor m/3\rfloor$ and recursively sort its first $m-k$ entries, its last $m-k$ entries, then its first $m-k$ entries again. Each child has length $\lceil2m/3\rceil$; the split must use the current subproblem length. The [master theorem](master-theorem.md) gives exponent $\log_{3/2}3\approx2.7095$, worse than quadratic. The usual algorithm is not stable: endpoint exchange on $[2_a,2_b,1]$ leaves the equal-key records reversed after sorting.

## ↑ Ancestors (4)

1. [Sorting algorithm](sorting-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms-resit/8/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms-resit/8/d/solution.md)
