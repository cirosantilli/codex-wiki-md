<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Given the target's current heap index $i$, remove it as follows. If $i=n$, discard the last entry. Otherwise replace $A[i]$ by $A[n]$ and reduce $n$ by one. If the replacement is larger than its [parent in a rooted tree](../../../../../parent-in-a-rooted-tree.md), use [sift up](../../../../../sift-up.md); otherwise use the maximum-oriented [sift down](../../../../../sift-down.md) from $i$.

Only comparisons incident to the replacement can initially violate the [heap order](../../../../../heap-order.md). If it exceeds its parent, it also dominates the old children because the old key dominated those children and was no larger than the parent; an upward repair suffices. Otherwise the upward comparison is valid and only a downward repair can be needed. Thus **removal takes $O(\log n)$ worst-case time** after the location is known. Searching an unindexed heap for an arbitrary specified key can instead require $\Theta(n)$ time; the logarithmic bound does not include such a search.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
