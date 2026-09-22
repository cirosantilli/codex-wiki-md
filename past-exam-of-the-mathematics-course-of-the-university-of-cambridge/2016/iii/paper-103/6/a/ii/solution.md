<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose an entry $y$ is bumped from column $j$ of row $i$. If row $i+1$ already contains a cell in column $j$, its entry is greater than $y$ by the strict column condition in the original [near Young tableau](../../../../../../../near-young-tableau.md). When $y$ is inserted into that row, the first entry greater than $y$ therefore occurs in a column at most $j$.

If the next row is shorter than $j$, either a bump occurs earlier or $y$ is appended in column $\lambda_{i+1}+1\leq j$. This also handles the final appended box. Each successive bumping position is therefore weakly to the left of the previous one. **The bumping columns satisfy**

$$
\boxed{j'\geq j''\geq j'''\geq\cdots}.
$$

This is the [row-insertion bumping-path monotonicity](../../../../../../../row-insertion-bumping-path-monotonicity.md) needed to preserve the Young-diagram shape and column order.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
