<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For finite [lists](../../../../../list-abstract-data-type.md) and $n\geq0$, the answers are
```
reverse (xs ++ ys) = reverse ys ++ reverse xs
length (drop n xs) = max 0 (length xs - n)
```
The maximum is necessary when the count exceeds the [list](../../../../../list-abstract-data-type.md) length.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
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
