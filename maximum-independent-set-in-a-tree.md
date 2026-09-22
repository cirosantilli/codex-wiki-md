# Maximum independent set in a tree

↑ **Parent:** [Maximum independent set](maximum-independent-set.md)

Root a finite [tree](tree-graph-theory-split.md). The two [dynamic programming](dynamic-programming.md) states are the optimal size in the descendant subtree when its root $v$ is included, $I(v)$, or excluded, $O(v)$. The sums run over its children. Inclusion forces every child to be excluded; exclusion permits each child's better state. Child subtrees have no edges between them, which proves independence of these choices. The leaf states are $I=1,O=0$, and the root's better state gives the optimum.

A [postorder traversal](postorder-traversal.md) computes the states in $O(n)$ time and storage. Reconstruct a set by following an attaining root choice and the same child constraints, breaking ties arbitrarily. The empty and singleton cases use the ordinary non-strict [subset](subset.md) convention.

## ↑ Ancestors (7)

1. [Maximum independent set](maximum-independent-set.md)
2. [Independent set (graph theory)](independent-set-graph-theory.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/6/e/solution.md)
