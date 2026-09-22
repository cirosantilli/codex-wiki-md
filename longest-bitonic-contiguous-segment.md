# Longest bitonic contiguous segment

↑ **Parent:** [Bitonic segment](bitonic-segment.md)

A [linear time](linear-time.md) scan can retain the earliest start of the current monotone suffix, the earliest start of the current bitonic suffix, the most recent nonzero direction and the endpoint of its most recent strict step. At a strict direction reversal, the new bitonic suffix begins at the old monotone start; the new monotone suffix begins at the old strict-step endpoint. Zero differences leave these boundaries unchanged. The suffix invariants show that no longer valid suffix is discarded, and recording the largest length gives a global optimum using constant auxiliary storage.

## ↑ Ancestors (5)

1. [Bitonic segment](bitonic-segment.md)
2. [Array (data structure)](array-data-structure.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming-resit/3/d/solution.md)
