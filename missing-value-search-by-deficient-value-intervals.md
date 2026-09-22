# Missing-value search by deficient value intervals

↑ **Parent:** [Binary search](binary-search.md)

Suppose a candidate [integer interval](integer-interval.md) contains $W$ possible values and an active [array](array-data-structure.md) segment contains exactly all occurrences from that interval, with $m<W$ entries. The [pigeonhole principle](pigeonhole-principle.md) guarantees a missing value. Split the value interval into widths $W_L,W_R$ and use [array partitioning](two-way-array-partition.md) to obtain occurrence counts $m_L,m_R$. If $m_L<W_L$, retain the left side. Otherwise $m_R=m-m_L<W-W_L=W_R$, so retain the right side. This works with duplicate entries because it needs only the inequality between occurrences and possible values.

Balancing the value widths gives $W_{i+1}\leq\lceil W_i/2\rceil$, while the active scan length remains less than $W_i$. The total work is bounded by a [geometric series](geometric-series.md) and logarithmic loop overhead, hence $O(W_0)$ [time complexity](time-complexity.md). On reaching width one, the retained occurrence count is zero, proving that the sole candidate is absent globally. This is a [binary search](binary-search.md) over deficient value intervals, with local in-place [array partitioning](two-way-array-partition.md), rather than repeated full-array scans.

## ↑ Ancestors (4)

1. [Binary search](binary-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/imperative-programming/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/2/c/solution.md)
