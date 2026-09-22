<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Java array](../../../../../../java-array.md) can hold references to row arrays. For example,
```
double[][] grid = new double[rows][columns];
grid[2][3] = 4.5;
```
allocates the outer array and all equal-length rows, with numeric entries initially zero. A ragged alternative is
```
double[][] grid = new double[rows][];
for (int r = 0; r < rows; r++)
    grid[r] = new double[r + 1];
```
The second form initially has null row references, so each row must be allocated before access. Rows need not have equal lengths, and a two-dimensional array of objects initially contains null object references rather than constructed cell objects. **Java represents a two-dimensional array as an array of arrays.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9](../../9.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
