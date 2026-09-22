<h1 id="12/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

To invert the [matrix](../../../../../../matrix.md), row-reduce the augmented [matrix](../../../../../../matrix.md) $(M\mid I)$. Subtracting row one from rows two and three gives left rows $(0,-4,1)$ and $(0,0,2)$, so the pivots are nonzero and back-substitution is possible. The resulting [matrix inverse](../../../../../../matrix-inverse-split.md) is

$$
\boxed{M^{-1}=\begin{pmatrix}
3/8&1/4&3/8\\1/8&-1/4&1/8\\-1/2&0&1/2
\end{pmatrix}}.
$$

Multiplying by $M$ verifies the identity [matrix](../../../../../../matrix.md). This inverse is not $M^T$; indeed

$$
M^TM=\begin{pmatrix}3&-1&0\\-1&11&0\\0&0&2\end{pmatrix}\ne I.
$$

Thus **$M$ is not [orthogonal](../../../../../../orthogonal-vectors.md)**.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [12](../../../12.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
