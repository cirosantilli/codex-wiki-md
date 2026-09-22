<h1 id="22h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose otherwise and choose linearly independent [eigenvectors](../../../../../../eigenvector.md) $v_n$ with $Tv_n=\lambda_nv_n$ and $|\lambda_n|>a$. Put $F_n=\operatorname{span}(v_1,\ldots,v_n)$. Each $F_n$ is finite-dimensional and $T$-invariant. Moreover $(T-\lambda_nI)F_n\subseteq F_{n-1}$, including when some [eigenvalues](../../../../../../eigenvalue.md) coincide.

Apply the supplied distance fact inside the [Banach space](../../../../../../banach-space-split.md) $F_n$ to choose $x_n\in F_n$ with $\|x_n\|=1$ and $\operatorname{dist}(x_n,F_{n-1})=1$. For $m<n$, both $(T-\lambda_nI)x_n$ and $Tx_m$ belong to $F_{n-1}$. Consequently

$$
\|Tx_n-Tx_m\|\ge \operatorname{dist}(\lambda_nx_n,F_{n-1})=|\lambda_n|>a.
$$

Thus $(Tx_n)$ has no Cauchy [subsequence](../../../../../../subsequence.md), although $(x_n)$ is bounded. This contradicts the [compact operator](../../../../../../compact-operator-split.md) property. **Only finitely many linearly independent [eigenvectors](../../../../../../eigenvector.md) can have [eigenvalue](../../../../../../eigenvalue.md) modulus greater than $a$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22H](../../22h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
