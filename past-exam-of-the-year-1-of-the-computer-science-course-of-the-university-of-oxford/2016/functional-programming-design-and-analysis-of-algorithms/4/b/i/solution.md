<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A recursive [transpose](../../../../../../transpose.md) removes the first column, then transposes the remaining columns:
```
transpose :: Matrix a -> Matrix a
transpose [] = []
transpose ([] : _) = []
transpose rows = map head rows : transpose (map tail rows)
```
The internal recursive calls eventually reach rows of length zero, even though the original input has positive dimensions; the second equation handles this terminating case. Rectangularity ensures that the rows become empty together, so no `head` or `tail` is applied to an empty row in the third equation. The output is **an $n\times m$ [matrix](../../../../../../matrix.md) with entry $b_{ji}=a_{ij}$**. The element type is unrestricted.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
