<h1 id="17/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

From part (f), $PQ=\operatorname{diag}(-1,-1,1)$. To obtain $PQR=-I$, choose the [Householder transformation](../../../../../householder-transformation.md) that reverses only the third coordinate:

$$
\boxed{R=\operatorname{diag}(1,1,-1),\qquad \mathbf r=(0,0,\sqrt2)^T.}
$$

Indeed $\mathbf r\mathbf r^T=\operatorname{diag}(0,0,2)$, so $R_{ij}=\delta_{ij}-r_ir_j$, and direct [matrix multiplication](../../../../../matrix-multiplication.md) gives $PQR=-I$. The alternative [vector](../../../../../vector.md) $-\mathbf r$ produces the same [matrix](../../../../../matrix.md). Geometrically $R$ reflects in the [plane](../../../../../plane.md) $x_3=0$, completing the reversal of all three coordinates.

## ↑ Ancestors (13)

1. [G](../g.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
