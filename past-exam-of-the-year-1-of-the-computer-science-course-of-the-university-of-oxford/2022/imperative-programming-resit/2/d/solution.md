<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume both dimensions are positive so the top-right entry exists. If **`f(0)(m-1) == x`**, it is already a match. If it is smaller than $x$, the entire first row is smaller, since it is that row's maximum; discard the first row. If it is larger than $x$, the entire last column is larger, since it is that column's minimum; discard the last column. This is the [staircase matrix search](../../../../../staircase-matrix-search.md) elimination step. Row and column monotonicity are both needed for the respective conclusions.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
