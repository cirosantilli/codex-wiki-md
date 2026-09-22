<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Build columns by prepending the first row's entries to the columns obtained from the remaining rows:
```
transpose :: Matrix a -> Matrix a
transpose [] = []
transpose [row] = map (:[]) row
transpose (row : rows) = zipWith (:) row (transpose rows)
```
The singleton case turns each entry into a one-element column. In the recursive case, `transpose rows` has exactly as many columns as `row` has entries, so `zipWith (:)` extends every column once. [Structural induction](../../../../../../structural-induction.md) on the number of rows proves that **each output column contains the corresponding input entries in order**. This uses [list zip](../../../../../../list-zip.md) to implement the [transpose](../../../../../../transpose.md), without requiring `Num a`.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
