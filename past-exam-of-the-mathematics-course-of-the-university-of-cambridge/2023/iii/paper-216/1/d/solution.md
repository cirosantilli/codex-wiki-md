<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the first $i$ observations, write

$$
A_i=\Sigma^{-1}+X_{1:i}^TX_{1:i},
\qquad b_i=X_{1:i}^TY_{1:i}.
$$

By [Gaussian conjugacy for a normal linear model](../../../../../../gaussian-conjugacy-for-a-normal-linear-model.md), the prefix posterior is

$$
\beta\mid Y_{1:i}\sim N(A_i^{-1}b_i,A_i^{-1}).
$$

Compute a [Cholesky decomposition](../../../../../../cholesky-decomposition.md) of $A_0=\Sigma^{-1}$ once. If $x_i^T$ is row $i$ of the [design matrix](../../../../../../design-matrix.md), then

$$
A_i=A_{i-1}+x_ix_i^T,
\qquad b_i=b_{i-1}+x_iY_i.
$$

The [Rank-one Cholesky update](../../../../../../rank-one-cholesky-update.md) obtains a triangular factor $A_i=L_iL_i^T$ from $L_{i-1}$ in $O(p^2)$ operations. Two [triangular solves](../../../../../../triangular-linear-system.md) give $m_i=A_i^{-1}b_i$, and, for $z_i\sim N(0,I_p)$, another solve gives

$$
\beta_i=m_i+L_i^{-T}z_i\sim N(m_i,A_i^{-1}).
$$

The initial factorization costs $O(p^3)$ and all $n$ updates and samples cost $O(np^2)$. This is within the requested $O(p^3+np^2+n^2p)$ bound.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
