# Minimum vertex cover of a tree

↑ **Parent:** [Minimum vertex cover](minimum-vertex-cover.md)

Root a finite [tree](tree-graph-theory-split.md), and let $D_0,D_1$ be the optimum [vertex cover](vertex-cover.md) sizes of a descendant [subtree](subtree.md) conditional on excluding or including its root. Excluding a parent forces all children to be included; including it permits either child state. These facts prove the displayed recurrences by [structural induction](structural-induction.md). Empty child sums give $D_0=0,D_1=1$ at a [leaf of a rooted tree](leaf-of-a-rooted-tree.md). Evaluating in [postorder traversal](postorder-traversal.md) and taking the smaller root state gives a linear-time [dynamic programming](dynamic-programming.md) algorithm.

## ↑ Ancestors (7)

1. [Minimum vertex cover](minimum-vertex-cover.md)
2. [Vertex cover](vertex-cover.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms/2/c/solution.md)
