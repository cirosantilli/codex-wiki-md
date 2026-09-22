# Red-black tree insertion

↑ **Parent:** [Red-black tree](red-black-tree.md)

In the usual bottom-up algorithm, insert a red node by the [binary search tree](binary-search-tree.md) rule. If its parent is black, no repair is needed. If its parent and uncle are red, recolour both black and recolour the grandparent red, then continue upward. If the uncle is black, an inner configuration first rotates the parent to become an outer configuration; rotating the grandparent and exchanging its colour with the parent's resolves the red-red conflict. Apply the left/right mirror cases as needed and finish with a black root. The [tree rotations](tree-rotation.md) preserve key order, and the colour changes preserve equal [black height](black-height.md). Different valid insertion conventions can produce different valid [red-black trees](red-black-tree.md), so a worked trace must identify its convention.

## ↑ Ancestors (6)

1. [Red-black tree](red-black-tree.md)
2. [Binary search tree](binary-search-tree.md)
3. [Binary tree](binary-tree.md)
4. [Data structure](data-structure-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms/1/d/solution.md)
