<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The first row has off-diagonal sum $a_{12}<1/4$. Rows $2,\ldots,n-1$ have sums less than $1/2$, and the last row has sum $c+a_{n,n-1}<5/4$, since $0<c<1$. Every row except the second therefore has its [Gershgorin disc](../../../../gershgorin-disc.md) strictly away from zero: its centre is at least one in the first row and at least three in the remaining rows.

For the second row, an exact sufficient condition is $|b|>a_{21}+a_{23}$. Since the sum is strictly below $1/2$, the coefficient-independent bounds

$$
\boxed{b\leq-\frac12\quad\text{or}\quad b\geq\frac12}
$$

guarantee that zero is outside every [Gershgorin disc](../../../../gershgorin-disc.md). Consequently zero is not an [eigenvalue](../../../../eigenvalue.md) and $A$ is an [invertible matrix](../../../../invertible-matrix.md). Equality at $\pm1/2$ is allowed because the off-diagonal entry bounds are strict. These are sufficient [strict diagonal dominance](../../../../strictly-diagonally-dominant-matrix.md) bounds; values of $b$ between them can also give invertible [matrices](../../../../matrix.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
