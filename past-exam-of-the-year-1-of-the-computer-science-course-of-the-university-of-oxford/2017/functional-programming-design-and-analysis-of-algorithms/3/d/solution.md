<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Enumerate assignments and retain exactly the valid completions:

```
solve :: Grid -> [Grid]
solve = filter complete . expand . choices
```

With $x$ blank cells and all other entries fixed, the unpruned [Cartesian product](../../../../../cartesian-product.md) has **$9^x$ candidate grids**. Testing `complete` enforces every row, column and box condition. This is the size of the full candidate search; [lazy evaluation](../../../../../lazy-evaluation.md) can stop earlier if the caller demands only an initial portion of the solution list.

## ↑ Ancestors (12)

1. [D](../d.md)
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
