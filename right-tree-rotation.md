# Right tree rotation

↑ **Parent:** [Tree rotation](tree-rotation.md)

For old root $y$ with left child $x$ and untouched [subtrees](subtree.md) $A,B,C$, change the shape from $((A,x,B),y,C)$ to $(A,x,(B,y,C))$. Both have inorder [sequence](sequence.md) $A,x,B,y,C$. In a destructive traversal that only rotates at the current root, this transformation extends the right spine by one node and decreases the left-size potential by one.

## ↑ Ancestors (5)

1. [Tree rotation](tree-rotation.md)
2. [Binary tree](binary-tree.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Destructive inorder traversal by right rotations](destructive-inorder-traversal-by-right-rotations.md)
- [Left-size potential of a binary tree](left-size-potential-of-a-binary-tree.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/1/f/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/1/g/solution.md)
