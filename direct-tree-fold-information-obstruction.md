# Direct tree-fold information obstruction

↑ **Parent:** [Tree fold](tree-fold.md)

A direct [tree fold](tree-fold.md) gives a parent operation only its children's folded summaries. If two different children have equal summaries, the parent cannot distinguish them. For a [leaf-labelled binary tree](leaf-labelled-binary-tree.md), a function returning proper [subtrees](subtree.md) maps every leaf to `[]`. A direct fold with precisely that result type would therefore map every two-leaf tree to the same result, despite their possibly different labels. This rules out that direct fold, while permitting a richer folded summary followed by projection.

## ↑ Ancestors (5)

1. [Tree fold](tree-fold.md)
2. [Functional programming](functional-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/1/h/solution.md)
