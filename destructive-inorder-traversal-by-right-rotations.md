# Destructive inorder traversal by right rotations

↑ **Parent:** [Inorder traversal](inorder-traversal.md)

While the remaining root has a left child, apply a [right tree rotation](right-tree-rotation.md) there. Once the left child is null, output the root and advance to its right child. The output already produced followed by the remaining inorder [sequence](sequence.md) is [invariant](invariant-mathematics.md). There are exactly $N$ output removals and $L(T_0)\leq N$ rotations, because rotations decrease the left-size potential and removals preserve it. The [algorithm](algorithm-split.md) therefore takes linear time and constant auxiliary pointer space, at the cost of changing the input links.

## ↑ Ancestors (5)

1. [Inorder traversal](inorder-traversal.md)
2. [Binary tree](binary-tree.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/1/f/solution.md)
