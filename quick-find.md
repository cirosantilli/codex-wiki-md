# Quick-find

↑ **Parent:** [Disjoint-set data structure](disjoint-set-data-structure.md)

An eager representation of a [disjoint-set data structure](disjoint-set-data-structure.md) that stores each member's current representative directly. Finding a representative is direct when keys are array indices; arbitrary keys in a parallel key array can add a [linear search](linear-search.md). A [disjoint-set union operation](disjoint-set-union-operation.md) scans members and replaces every occurrence of one old representative with the other. The representative labels must be snapshotted before this scan. Its easy [abstraction function](abstraction-function.md) contrasts with the parent-pointer representation of a [disjoint-set forest](disjoint-set-forest.md).

## ↑ Ancestors (4)

1. [Disjoint-set data structure](disjoint-set-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/5/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/5/e/solution.md)
- [Snapshot representatives before quick-find union](snapshot-representatives-before-quick-find-union.md)
