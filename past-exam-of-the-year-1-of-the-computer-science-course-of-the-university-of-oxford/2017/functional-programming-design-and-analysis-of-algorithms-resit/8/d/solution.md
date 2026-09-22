<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Prefer the alternatives for large unrestricted arrays.** [Merge sort](../../../../../merge-sort.md) and [heapsort](../../../../../heapsort.md) have $O(n\log n)$ worst-case time, while [insertion sort](../../../../../insertion-sort.md) has $O(n^2)$ worst-case time and can be much faster on nearly sorted data. The intended [stooge sort](../../../../../stooge-sort.md) has worst-case $\Theta(n^{2.7095\ldots})$, so even insertion sort has the better worst-case exponent.

The first two give the stronger general asymptotic guarantee. Choices between them can depend on storage and [stable sorting](../../../../../stable-sorting.md) requirements; these considerations do not rescue Stooge sort's much larger work count.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
