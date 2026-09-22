<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [merge sort](../../../../../merge-sort.md): recursively sort the left and right halves of the [array](../../../../../array-data-structure.md), then merge their ordered outputs using two advancing indices. A merge reads or writes each element a constant number of times, so it costs $O(n)$. There are $O(\log n)$ balanced recursion levels with $O(n)$ total work per level. Hence the worst-case running time is **$O(n\log n)$**; the standard array implementation uses $O(n)$ auxiliary storage.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
