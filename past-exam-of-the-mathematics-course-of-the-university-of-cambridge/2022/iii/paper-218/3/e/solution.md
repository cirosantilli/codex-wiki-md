<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For fixed $A$, differentiating under the constraint $\sum_i z_i=0$ gives

$$
\widehat\mu=\overline X,
\qquad
\widehat z_i=(A^TA)^{-1}A^T(X_i-\overline X).
$$

Because the columns $u_j$ are orthogonal,

$$
\widehat z_{ij}
=\frac{u_j^T(X_i-\overline X)}{\|u_j\|_2^2}.
$$

The fitted value is therefore $\overline X+\Pi_A(X_i-\overline X)$, where $\Pi_A$ is the [orthogonal projection](../../../../../../orthogonal-projection.md) onto the column space of $A$.

The residual sum of squares is minimized by choosing this column space to be the span of the $d$ leading eigenvectors of

$$
\sum_i(X_i-\overline X)(X_i-\overline X)^T.
$$

**Thus $\widehat A$ may be taken to have those orthonormal eigenvectors as columns. Their nonzero scales are immaterial because inverse scaling of the scores leaves $Az_i$ unchanged.**

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
