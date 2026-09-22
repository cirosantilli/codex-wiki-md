<h1 id="6/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Store a [complete binary tree](../../../../../../complete-binary-tree.md) in a one-indexed [array](../../../../../../array-data-structure.md) $A[1..n]$, level by level. Index $i$ has [parent in a rooted tree](../../../../../../parent-in-a-rooted-tree.md) $\lfloor i/2\rfloor$ for $i>1$ and possible [children in a rooted tree](../../../../../../child-in-a-rooted-tree.md) $2i$ and $2i+1$, present only when their indices are at most $n$. The [max-heap](../../../../../../max-heap.md) condition is $A[\lfloor i/2\rfloor]\ge A[i]$ for every $i>1$.

Following these inequalities from the [root of a tree](../../../../../../root-of-a-tree.md) to any entry proves that **$A[1]$ is a [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md)**. The [heap order](../../../../../../heap-order.md) does not sort siblings or unrelated branches. The [complete binary tree](../../../../../../complete-binary-tree.md) has height $\lfloor\log_2 n\rfloor$, which bounds how far any single repair can travel. Store the current heap size separately from the [array](../../../../../../array-data-structure.md)'s capacity.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
