<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [singular value system](../../../../../../singular-system-of-a-compact-operator.md) of a [compact operator](../../../../../../compact-operator-split.md) consists of positive numbers $\sigma_j$ and orthonormal families $v_j\in X$, $u_j\in Y$ satisfying

$$
\boxed{Av_j=\sigma_j u_j,\qquad A^*u_j=\sigma_jv_j.}
$$

Thus $v_j$ are positive-eigenvalue [eigenvectors](../../../../../../eigenvector.md) of $A^*A$ and $u_j$ of $AA^*$, with [eigenvalue](../../../../../../eigenvalue.md) $\sigma_j^2$. The families are complete in $(\ker A)^\perp$ and $\overline{\operatorname{ran}A}$ respectively. The [singular values](../../../../../../singular-value.md) can be listed nonincreasingly with multiplicities, and tend to zero in the infinite-rank case. For finite rank there are only finitely many positive [singular values](../../../../../../singular-value.md); zero-kernel directions are handled separately.

Use the convention that $\langle f,g\rangle$ is conjugate-linear in its first entry. Then the [singular value system](../../../../../../singular-system-of-a-compact-operator.md) gives

$$
Ax=\sum_j\sigma_j u_j\langle v_j,x\rangle,\qquad A^\dagger y=\sum_j\frac{\langle u_j,y\rangle}{\sigma_j}v_j.
$$

The latter series converges precisely on the admissible range component specified by the [Picard criterion](../../../../../../picard-criterion.md):

$$
\sum_j\frac{|\langle u_j,y\rangle|^2}{\sigma_j^2}<\infty,
$$

with $R^\perp$ components annihilated by the inverse. Merely writing a formal singular expansion does not imply it converges in $X$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
