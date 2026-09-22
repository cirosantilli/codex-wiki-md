<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

The [Jordan normal form](../../../../../jordan-normal-form.md) theorem says that every complex square [matrix](../../../../../matrix.md) is similar to a direct sum of Jordan blocks, uniquely up to their order. For an [eigenvalue](../../../../../eigenvalue.md) $\lambda$, if its blocks have sizes $n_1,\ldots,n_r$, then its [algebraic multiplicity](../../../../../algebraic-multiplicity.md) and [geometric multiplicity](../../../../../geometric-multiplicity.md) are

$$
a_\lambda=\sum_{j=1}^r n_j,
\qquad
g_\lambda=r,
$$

and its contribution to the [minimal polynomial](../../../../../minimal-polynomial.md) is $(t-\lambda)^{\max_j n_j}$. Thus

$$
m_\alpha(t)=\prod_\lambda(t-\lambda)^{s_\lambda},
$$

where $s_\lambda$ is the largest $\lambda$-block size.

For the given [matrix](../../../../../matrix.md),

$$
\det(tI-A)=(t-2)(t+1)^2.
$$

Moreover,

$$
\dim\ker(A-2I)=1,
\qquad
\dim\ker(A+I)=1.
$$

Hence

$$
\boxed{a_2=g_2=1,
\qquad a_{-1}=2,
\qquad g_{-1}=1}.
$$

The [eigenvalue](../../../../../eigenvalue.md) $-1$ therefore has one Jordan block of size two, so

$$
\boxed{m_\alpha(t)=(t-2)(t+1)^2}.
$$

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
