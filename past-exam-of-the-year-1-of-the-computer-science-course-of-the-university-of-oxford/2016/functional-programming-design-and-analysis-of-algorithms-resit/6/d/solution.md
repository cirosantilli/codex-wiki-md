<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [counting sort](../../../../../counting-sort.md) with 26 counters, indexed by the character code minus the code for `A`. Scan the input to obtain each character's count, then emit that many copies in alphabetic order. Counting costs $O(n)$; visiting 26 counters and writing $n$ outputs costs $O(n+26)=O(n)$.

The comparison lower bound does not apply because the algorithm uses a fixed-size known alphabet and direct key indexing. It does not have to distinguish $n!$ distinct-key orders by binary comparisons; for $n>26$, distinctness is not even possible in this alphabet.

## ↑ Ancestors (12)

1. [D](../d.md)
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
