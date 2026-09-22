# Perfect rose tree

↑ **Parent:** [Rose tree](rose-tree.md)

A [rose tree](rose-tree.md) is perfect when all its [leaves of a rooted tree](leaf-of-a-rooted-tree.md) have the same depth. This permits unequal branching counts and unary branches; perfectness alone does not require every internal [vertex](vertex-graph-theory.md) to have the same number of children. A bottom-up certificate returns `Just 0` at a leaf, `Just (h+1)` when all child certificates are `Just h`, and `Nothing` otherwise. [Structural induction](structural-induction.md) proves that a certificate exists exactly when the tree is perfect: all root-to-leaf routes acquire one edge when attached to the new root.

## ↑ Ancestors (7)

1. [Rose tree](rose-tree.md)
2. [Rooted tree](rooted-tree.md)
3. [Tree (graph theory)](tree-graph-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/2/b/solution.md)
