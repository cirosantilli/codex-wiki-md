# Explicit-stack depth-first tree traversal

↑ **Parent:** [Depth-first search](depth-first-search.md)

An [explicit-stack depth-first tree traversal](explicit-stack-depth-first-tree-traversal.md) stores pending subtree roots instead of suspended recursive calls. In a [binary tree](binary-tree.md), visit the current node, defer its nonempty right child on a [stack](stack-data-structure.md), and continue with its left child; pop when the current subtree is empty. The unvisited subtrees remain disjoint and, together with the visited nodes, partition the original tree. This [loop invariant](loop-invariant.md) proves that accumulating each visited label gives the tree sum. At most one right sibling per ancestor is pending, so auxiliary storage is $O(d)$ for depth $d$ and running time is $\Theta(N)$ for $N$ nodes. Unlike a full recursive [stack frame](stack-frame.md), a pending entry need contain only a subtree [pointer](pointer-computer-programming.md).

## ↑ Ancestors (4)

1. [Depth-first search](depth-first-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Explicit-stack depth-first tree traversal](explicit-stack-depth-first-tree-traversal.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/d/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/4/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/1/b/solution.md)
