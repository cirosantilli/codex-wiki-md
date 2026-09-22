# Leaf-labelled binary tree

↑ **Parent:** [Binary tree](binary-tree.md)

A [binary tree](binary-tree.md) with each data label stored at a [leaf of a tree](leaf-of-a-tree.md). One useful [Haskell](haskell.md) datatype has constructors `One a` for a leaf and `Two (Tree a) (Tree a)` for an internal node. Every finite inhabitant has at least one leaf, so this datatype cannot encode an empty leaf sequence. Its natural [tree fold](tree-fold.md) has a leaf operation `a -> b` and an internal operation `b -> b -> b`; replacing the two constructors by those operations defines the [structural recursion](structural-recursion.md).

## ↑ Ancestors (4)

1. [Binary tree](binary-tree.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Algebraic data type](algebraic-data-type.md)
- [Direct tree-fold information obstruction](direct-tree-fold-information-obstruction.md)
- [Leaf-balanced binary tree](leaf-balanced-binary-tree.md)
- [Linear flattening of a binary tree](linear-flattening-of-a-binary-tree.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/2/c/solution.md)
- [Tree fold](tree-fold.md)
