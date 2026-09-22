<h1 id="8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**No: Stooge sort is not stable.** Give equal keys distinct record identities and start with

$$
[2_a,2_b,1].
$$

The initial endpoint swap gives $[1,2_b,2_a]$. The later two-element calls either see increasing keys or equal keys, so they make no swap. The two records with key 2 have reversed their original order, contradicting [stable sorting](../../../../../stable-sorting.md). The example uses length three, where the intended current-length split is unambiguous.

## ↑ Ancestors (12)

1. [E](../e.md)
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
