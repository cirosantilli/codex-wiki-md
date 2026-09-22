# Tree fold

↑ **Parent:** [Functional programming](functional-programming.md)

A [structural recursion](structural-recursion.md) replacing the empty binary tree by a value and a nonempty node by a combining function on its two folded children and root label. The result type may itself be a [function type](function-type.md), allowing a fold to construct a membership [predicate](predicate.md) or a [difference list](difference-list.md) rather than traversing all branches for every subsequent query.

More generally, choose one operation for each [data constructor](data-constructor.md). For a [leaf-labelled binary tree](leaf-labelled-binary-tree.md) represented by `One a | Two (Tree a) (Tree a)`, the [tree fold](tree-fold.md) instead has [type signature](type-signature.md) `(a -> b) -> (b -> b -> b) -> Tree a -> b`: one operation handles the leaf label, and the other combines the two folded children. Replacing the operations by the original [data constructors](data-constructor.md) reconstructs the input, as [structural induction](structural-induction.md) proves.

**Table of contents**

- [Direct tree-fold information obstruction](direct-tree-fold-information-obstruction.md)

## ↑ Ancestors (4)

1. [Functional programming](functional-programming.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (26)

- [Difference list](difference-list.md)
- [Direct tree-fold information obstruction](direct-tree-fold-information-obstruction.md)
- [Leaf-labelled binary tree](leaf-labelled-binary-tree.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/4/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/4/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/4/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/4/f/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/d/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/3/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/1/f/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/1/h/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/2/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/functional-programming-design-and-analysis-of-algorithms-resit/2/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/4/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/4/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/4/g/solution.md)
- [Predicate](predicate.md)
- [Rose tree](rose-tree.md)
- [Tree fold](tree-fold.md)
- [Undoing insertion of a new extreme key](undoing-insertion-of-a-new-extreme-key.md)
