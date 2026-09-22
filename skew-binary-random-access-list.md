# Skew-binary random-access list

↑ **Parent:** [Random-access list](random-access-list.md)

Represent a finite [list](list-abstract-data-type.md) by a [forest](forest.md) of value-bearing [perfect binary trees](perfect-binary-tree.md) of sizes $1,3,7,\ldots$, in nondecreasing order, using the greedy largest sizes and allowing a repeated size only in the first two positions. Concatenated [preorder traversals](preorder-traversal.md) recover the [list](list-abstract-data-type.md). Cached tree sizes guide indexing.

Front insertion merges the first two equal-size trees beneath a new root, or adds a singleton if they differ. Removing the first root either discards a singleton or splits its two children into the initial equal-size pair. Both operations inspect and allocate only a bounded number of constructors, taking worst-case [constant time](constant-time.md) and sharing the remaining representation. A positional query skips whole cached tree sizes and then descends through one tree, taking $O(\log(n+1))$ time. Conversion in either direction takes [linear time](linear-time.md) on finite input.

The duplicate-size restriction follows directly from greediness. If two size-$w$ trees had any preceding nonempty portion, there would be at least $2w+1$ elements available, enough for the next larger [perfect binary tree](perfect-binary-tree.md). Three equal-size trees would likewise suffice for that larger tree. Both contradict the greedy representation.

## ↑ Ancestors (5)

1. [Random-access list](random-access-list.md)
2. [List (abstract data type)](list-abstract-data-type.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/2/f/solution.md)
- [Random-access list](random-access-list.md)
