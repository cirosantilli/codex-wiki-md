# Leaf-balanced binary tree

↑ **Parent:** [Balanced binary tree](balanced-binary-tree.md)

A [leaf-labelled binary tree](leaf-labelled-binary-tree.md) is leaf-balanced when the leaf counts of the two subtrees at every internal node differ by at most one. Splitting a finite nonempty [list](list-abstract-data-type.md) into pieces of sizes $\lfloor n/2\rfloor$ and $\lceil n/2\rceil$ and applying the same construction recursively preserves the original leaf order and gives this balance condition. Both pieces are nonempty for $n\ge2$ and strictly shorter than the input; [induction](mathematical-induction.md) proves termination and balance. This leaf-count convention is different from demanding equal subtree heights.

## ↑ Ancestors (5)

1. [Balanced binary tree](balanced-binary-tree.md)
2. [Binary tree](binary-tree.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/2/f/solution.md)
