# Diagonal merging of lazy lists

↑ **Parent:** [Fair enumeration](fair-enumeration.md)

For an outer [proper lazy list](proper-lazy-list.md) of inner [proper lazy lists](proper-lazy-list.md), introduce row $i$ in round $i$ and advance each active row once per round. Discard an active row when its terminating constructor is observed. Each round inspects finitely many rows, and the entry at row index $i$, within-row index $j$, is emitted in round $i+j$. Every earlier round has finite work, proving [fair enumeration](fair-enumeration.md) of all occurrences.

An implementation can keep a finite [list](list-abstract-data-type.md) of row remainders, append at most one newly introduced row, collect one head from every nonempty remainder, and retain their tails for the next round. It must not first combine all not-yet-introduced rows. In fact, `foldr interleave [] ([1,2] : repeat [])` can emit `1` and then block before `2`; [diagonal merging of lazy lists](diagonal-merging-of-lazy-lists.md) emits both. If infinitely many empty rows remain after the final output, detecting termination is impossible in general: the [absence-detection obstruction for infinite lists](absence-detection-obstruction-for-infinite-lists.md) prevents a universal promise of a terminating empty tail, while every required occurrence can still be emitted.

## ↑ Ancestors (4)

1. [Fair enumeration](fair-enumeration.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Diagonal merging of lazy lists](diagonal-merging-of-lazy-lists.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/3/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/4/d/solution.md)
