<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Maintaining strictly decreasing powers makes output deterministic and avoids sorting a copy at every print. More significantly, two sorted sparse polynomials can be added by a [merge algorithm](../../../../../merge-algorithm.md) in **$O(m+n)$ time**, combining equal powers and dropping cancellations as they are encountered.

The cost is maintaining that order during construction and updates. A linked-list insertion can require a linear search, while initially sorting $t$ unsorted terms costs $O(t\log t)$ comparisons before combining duplicates. Multiplication still has to generate and combine term products; sorted storage does not make it linear automatically, though it enables merging ordered partial products. Keeping the invariant is attractive when arithmetic and printing are frequent; sorting only when printing can be simpler for infrequently displayed, frequently appended data.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [4](../../4.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
