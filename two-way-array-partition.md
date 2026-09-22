# Two-way array partition

↑ **Parent:** [Algorithm](algorithm-split.md)

Rearrange an [array](array-data-structure.md) segment $a[l,r)$ into a low segment containing values below a pivot $p$ and a high segment containing values at least $p$, preserving the segment's [multiset](multiset.md) and leaving the rest of the [array](array-data-structure.md) unchanged. The pivot need not itself occur, and either resulting segment may be empty.

An in-place scan maintains indices $l\leq k\leq j\leq r$ with $a[l,k)<p$ and $a[k,j)\geq p$. A low value at $j$ is swapped into position $k$ and advances both indices; a high value advances only $j$. The unexamined length $r-j$ is a [loop variant](loop-variant.md). At exit $j=r$, establishing the separation in $\Theta(r-l+1)$ [time complexity](time-complexity.md) and $O(1)$ auxiliary [space complexity](space-complexity.md). Equal values consistently belong to the high side.

**Table of contents**

- [Three-way array partitioning](three-way-array-partitioning.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/4/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/4/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/2/c/solution.md)
