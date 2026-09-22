<h1 id="15g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose an invertible change-of-basis [matrix](../../../../../../matrix.md) $P$ so that $J=PTP^{-1}$ is the [Jordan normal form](../../../../../../jordan-normal-form.md) of $T$. Write each block as

$$
J_{m_j}(\lambda_j)=\lambda_jI_{m_j}+N_{m_j},
$$

where $N_{m_j}$ has ones on its first superdiagonal and all other entries zero. Define

$$
D_0=\bigoplus_j\lambda_jI_{m_j},\qquad N=\bigoplus_jN_{m_j}.
$$

Every $\lambda_j\ne0$ because $T$ is invertible, so $D_0$ is an invertible [diagonal matrix](../../../../../../diagonal-matrix.md). The [matrix](../../../../../../matrix.md) $N$ is strictly upper triangular and hence nilpotent. On each block $D_0$ is a scalar multiple of the identity, so it commutes with $N$ on that block and therefore on the whole space. This gives

$$
\boxed{PTP^{-1}=D_0+N,\qquad D_0N=ND_0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15G](../../15g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
