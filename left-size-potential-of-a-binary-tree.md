# Left-size potential of a binary tree

↑ **Parent:** [Binary tree](binary-tree.md)

Define $L(\varnothing)=0$ and $L(T)=|T.left|+L(T.right)$. Subtracting the right-spine length from total size gives the same quantity, because every node lies either on that spine or in one of its disjoint left [subtrees](subtree.md). A [right tree rotation](right-tree-rotation.md) at the root decreases this potential by exactly one; removing a root with no left child preserves it. Thus repeated root rotations and inorder removals take linear total work.

## ↑ Ancestors (4)

1. [Binary tree](binary-tree.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/1/g/solution.md)
