# Sift down

↑ **Parent:** [Binary heap](binary-heap.md)

To repair a key in a minimum-oriented [binary heap](binary-heap.md), choose the smaller-priority present entry among its [children in a rooted tree](child-in-a-rooted-tree.md). Exchange if that entry is smaller than the moving key, and continue at the new index. Stop when there are no [children in a rooted tree](child-in-a-rooted-tree.md) or the [heap order](heap-order.md) holds. The smaller [rooted trees](rooted-tree.md) below the starting entry must already obey the [heap order](heap-order.md); choosing the larger child could leave a violation with the smaller one.

## ↑ Ancestors (5)

1. [Binary heap](binary-heap.md)
2. [Priority queue](priority-queue.md)
3. [Data structure](data-structure.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Binary heap](binary-heap.md)
