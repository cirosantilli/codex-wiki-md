# Splaying

↑ **Parent:** [Splay tree](splay-tree.md)

In ordinary bottom-up [splaying](splaying.md), locate the selected node by a [binary search tree](binary-search-tree.md) search and repeatedly move it toward the root. If its parent is the root, perform a [zig step](zig-step.md). Otherwise use a [zig-zig step](zig-zig-step.md) when the node and its parent occupy the same left/right directions, or a [zig-zag step](zig-zag-step.md) when their directions differ. Each [tree rotation](tree-rotation.md) preserves the [inorder traversal](inorder-traversal.md) and hence the represented key order. The process ends with the selected key at the root. Unsuccessful access policies can instead move the last visited node to the root; arguments about successful calls should say the requested key exists.

**Table of contents**

- [Splaying a chosen node into a leaf](splaying-a-chosen-node-into-a-leaf.md)
- [Zig-zag step](zig-zag-step.md)
- [Zig-zig step](zig-zig-step.md)
- [Zig step](zig-step.md)

## ↑ Ancestors (6)

1. [Splay tree](splay-tree.md)
2. [Binary search tree](binary-search-tree.md)
3. [Binary tree](binary-tree.md)
4. [Data structure](data-structure-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Consecutive keys in a binary search tree](consecutive-keys-in-a-binary-search-tree.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms/1/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms/1/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms/1/f/solution.md)
- [Splay tree](splay-tree.md)
- [Splaying](splaying.md)
- [Splaying a chosen node into a leaf](splaying-a-chosen-node-into-a-leaf.md)
