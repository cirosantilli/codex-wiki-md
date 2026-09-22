# Quickselect

↑ **Parent:** [Selection algorithm](selection-algorithm.md)

A [selection algorithm](selection-algorithm.md) that uses [array partitioning](two-way-array-partition.md) around a pivot and recursively searches only the side containing the desired [order statistic](order-statistic.md). If there are $s$ entries before the placed pivot, an earlier rank is unchanged and a later rank is reduced by $s+1$. Segment length strictly decreases, proving [algorithm termination](algorithm-termination.md). The same reduction can update local bounds in a loop, using constant auxiliary space.

Balanced reductions give linear work by a [geometric series](geometric-series.md), while repeatedly discarding only a constant number of entries can give quadratic work. For distinct entries and independent uniform random pivots, a pivot in the middle half has probability at least one half and reduces the retained length to at most three quarters, up to rounding. The expected number of attempts for each such reduction is bounded, so summing expected work over geometric size scales gives $O(n)$ expected time. This random-pivot guarantee is not a worst-case guarantee for a deterministic median-of-three heuristic. With duplicates and a strict two-way partition, random pivot choice alone can also fail to shrink an all-equal segment; a three-way partition treats equal keys together.

**Table of contents**

- [Median-of-three pivot selection](median-of-three-pivot-selection.md)
  - [Quadratic median-of-three selection family](quadratic-median-of-three-selection-family.md)

## ↑ Ancestors (4)

1. [Selection algorithm](selection-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/6/c/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/4/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/2/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming/2/e/solution.md)
- [Quadratic median-of-three selection family](quadratic-median-of-three-selection-family.md)
- [Three-way array partitioning](three-way-array-partitioning.md)
