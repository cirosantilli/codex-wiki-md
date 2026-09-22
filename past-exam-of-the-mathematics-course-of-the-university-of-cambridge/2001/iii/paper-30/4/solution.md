<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [balanced incomplete block design](../../../../../balanced-incomplete-block-design.md) has $t$ treatments and $b$ blocks, each containing $k$ distinct treatments with $1<k<t$. Every treatment occurs in $r$ blocks and every distinct treatment pair occurs together in $\lambda>0$ blocks. A [symmetric balanced incomplete block design](../../../../../symmetric-balanced-incomplete-block-design.md) has $b=t$, which implies $r=k$ by the first counting identity below.

For the separate even-order condition, let $N$ be the square treatment-by-block [incidence matrix of a set system](../../../../../incidence-matrix-of-a-set-system.md) of a symmetric design. Its diagonal overlap counts are $r$ and its off-diagonal counts are $\lambda$, giving

$$
NN^T=(r-\lambda)I+\lambda J.
$$

The counting identities proved in the next slots show that $r=k$ and $r+(t-1)\lambda=r^2$. Consequently the [eigenvalues](../../../../../eigenvalue.md) of $NN^T$ are $r^2$ on the constant vector and $r-\lambda$ on its $(t-1)$-dimensional orthogonal complement. Taking [determinants](../../../../../determinant.md) gives

$$
\det(N)^2=r^2(r-\lambda)^{t-1}.
$$

If $b=t$ is even, the exponent $t-1$ is odd. The exponent of every prime in $\det(N)^2$ and in $r^2$ is even; therefore its exponent in the positive integer $r-\lambda$ must be even. This proves the [even-order symmetric design square obstruction](../../../../../even-order-symmetric-design-square-obstruction.md):

$$
\boxed{r-\lambda\text{ is a perfect square}.}
$$

It is a necessary condition, not a sufficiency claim.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
