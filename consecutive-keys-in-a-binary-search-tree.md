# Consecutive keys in a binary search tree

↑ **Parent:** [Binary search tree](binary-search-tree.md)

Two stored keys $a<b$ are consecutive when no stored key lies strictly between them. Their numerical difference need not be one. After [splaying](splaying.md) on $a$ followed by [splaying](splaying.md) on $b$, the node $a$ is the left child of $b$ with an empty right [subtree](subtree.md). To prove this, after the first call $b$ is the minimum of the right [subtree](subtree.md) of $a$. The last step crossing $a$ is either a [zig step](zig-step.md) or a right-left [zig-zag step](zig-zag-step.md); both make $a$ the left child of $b$. A nonempty right [subtree](subtree.md) of $a$ would require a stored key strictly between them.

## ↑ Ancestors (5)

1. [Binary search tree](binary-search-tree.md)
2. [Binary tree](binary-tree.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms/1/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms/1/f/solution.md)
- [Splaying a chosen node into a leaf](splaying-a-chosen-node-into-a-leaf.md)
