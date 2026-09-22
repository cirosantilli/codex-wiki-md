# Structural sharing

↑ **Parent:** [Persistent data structure](persistent-data-structure.md)

Different immutable versions reuse unchanged component [software objects](software-object.md) rather than duplicating them. Sharing a [linked list](linked-list.md) suffix or unchanged [subtrees](subtree.md) saves storage while retaining distinct roots. The shared components must remain immutable for old versions to remain trustworthy. Merely sharing a mutable [array](array-data-structure.md) does not create a stable snapshot.

Saving references to before/after versions adds constant reference storage per history entry, but the data reachable through those references may be much larger. With balanced-tree path copying, $h$ small updates to a size-$n$ structure can retain $O(n+h\log n)$ nodes. Whole-array copying can instead retain $\Theta(hn)$ entries. The implementation and update pattern determine which bound applies.

## ↑ Ancestors (4)

1. [Persistent data structure](persistent-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/8/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/6/c/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/6/c/ii/solution.md)
