# Linear flattening of a binary tree

↑ **Parent:** [Difference list](difference-list.md)

For a [leaf-labelled binary tree](leaf-labelled-binary-tree.md), define `go (One x) acc = x:acc` and `go (Two l r) acc = go l (go r acc)`, then apply `go t []`. The invariant in the title follows by [structural induction](structural-induction.md) and [associativity](associative-property.md) of [list concatenation](list-concatenation.md). It proves preservation of leaf order. Each leaf supplies one output constructor and each internal node requires constant bookkeeping, giving [linear time](linear-time.md) in the number of nodes. By contrast, flattening both subtrees and concatenating their results can copy prefixes of sizes $1,2,\ldots,n-1$ on a left-branching [tree](tree-graph-theory-split.md), taking [quadratic time](quadratic-time.md). The accumulator is the already-known suffix in a [difference list](difference-list.md) representation.

## ↑ Ancestors (5)

1. [Difference list](difference-list.md)
2. [List (abstract data type)](list-abstract-data-type.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Concatenation tree](concatenation-tree.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/3/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/2/e/solution.md)
