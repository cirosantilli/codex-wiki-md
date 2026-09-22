<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First enumerate each possible row, then choose one row from each row's alternatives:

```
expand :: Matrix [a] -> [Matrix a]
expand = cp . map cp
```

The inner [Cartesian product](../../../../../cartesian-product.md) converts one row of cell choices into its possible rows; the outer product combines those rows into whole [matrices](../../../../../matrix.md). Every assignment is represented exactly once when each cell's alternatives are distinct. Empty cell domains yield no grids, and an empty matrix yields the singleton list containing the empty matrix.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
