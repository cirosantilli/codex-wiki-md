<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Retaining the estimator exactly as printed, define the probability limit

$$
c=\frac{\mathbb E[ZX]}{\mathbb E[Z^2]},
\qquad W=Z-cX.
$$

The empirical equations are linear in $(\beta,\alpha)$. Their coefficient matrix converges to

$$
M=
\begin{pmatrix}
\mathbb E[AW]&\mathbb E[XW]\\
\mathbb E[AX]&\mathbb E[X^2]
\end{pmatrix}.
$$

Therefore a sufficient condition, requiring neither parametric assumption, is

$$
0<\mathbb E[Z^2]<\infty,
\qquad
\det M
=\mathbb E[AW]\mathbb E[X^2]
-\mathbb E[XW]\mathbb E[AX]\ne0,
$$

with finite moments sufficient for the [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md). The empirical determinant then converges to a nonzero number, so the two linear equations have a unique solution with probability tending to one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
