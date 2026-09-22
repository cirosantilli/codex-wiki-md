# Rose tree

↑ **Parent:** [Rooted tree](rooted-tree.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rose_tree)

A [rose tree](rose-tree.md) is an ordered [rooted tree](rooted-tree.md) in which each [vertex](vertex-graph-theory.md) can have any finite number of [children in a rooted tree](child-in-a-rooted-tree.md). A labelled [Haskell](haskell.md) representation is `data RTree a = Node a [RTree a]`. Its [tree fold](tree-fold.md) has type `(a -> [b] -> b) -> RTree a -> b`: recursively fold the children, then combine their results with the current label. Unlike a [binary tree](binary-tree.md), a rose tree has no fixed pair of child positions.

**Table of contents**

- [Perfect rose tree](perfect-rose-tree.md)

## ↑ Ancestors (6)

1. [Rooted tree](rooted-tree.md)
2. [Tree (graph theory)](tree-graph-theory-split.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/3/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/d/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/d/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/d/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/2/c/solution.md)
- [Perfect rose tree](perfect-rose-tree.md)
- [Perfect ternary tree](perfect-ternary-tree.md)
- [Rose tree](rose-tree.md)
