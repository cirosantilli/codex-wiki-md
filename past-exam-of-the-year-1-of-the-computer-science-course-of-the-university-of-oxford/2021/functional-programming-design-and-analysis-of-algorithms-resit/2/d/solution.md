<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**`toTree` needs `Ord a`; `fromTree` does not.** Construction compares each key against a pivot. Flattening merely traverses and concatenates the buckets, so its more general type is `Tree a -> [a]`. A manually constructed tree need not satisfy the search-tree [invariant](../../../../../invariant-mathematics.md); `fromTree` still flattens it, although its output need not be sorted.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
