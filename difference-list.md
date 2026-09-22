# Difference list

↑ **Parent:** [List (abstract data type)](list-abstract-data-type.md)

Represent a [list](list-abstract-data-type.md) $xs$ by the [function](function-split.md) `\ys -> xs ++ ys`. Concatenation becomes function composition, the empty list is represented by `id`, and applying to `[]` recovers the list. Only functions of this tail-prepending form are valid representations; arbitrary functions of the displayed type need not satisfy the invariant. A higher-order [tree fold](tree-fold.md) using difference lists produces an inorder traversal in linear time on every tree shape.

**Table of contents**

- [Linear flattening of a binary tree](linear-flattening-of-a-binary-tree.md)

## ↑ Ancestors (4)

1. [List (abstract data type)](list-abstract-data-type.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Linear flattening of a binary tree](linear-flattening-of-a-binary-tree.md)
- [List concatenation](list-concatenation.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/3/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/2/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/4/b/solution.md)
- [Tree fold](tree-fold.md)
