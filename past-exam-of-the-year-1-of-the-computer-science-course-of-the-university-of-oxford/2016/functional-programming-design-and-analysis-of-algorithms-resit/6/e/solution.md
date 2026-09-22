<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For bare characters, equal occurrences are indistinguishable. The count-and-reconstruct implementation in (d) nevertheless **does not preserve the identities of equal-key records**, and so cannot provide [stable sorting](../../../../../stable-sorting.md) of associated payloads.

A stable refinement computes cumulative counts $C[j]$, the number of input keys at most $j$, then scans the original records right to left. For a record with key $j$, decrement $C[j]$ and place the complete record at output index $C[j]$. Equal-key records are placed from the end of their allocated range in reverse scanning order, preserving their original relative order. This costs $O(n+26)$ time and $O(n+26)$ auxiliary storage.

## ↑ Ancestors (12)

1. [E](../e.md)
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
