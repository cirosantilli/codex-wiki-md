<h1 id="11e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose an [orthonormal basis](../../../../../../orthonormal-basis.md) of eigenvectors of the [positive-definite operator](../../../../../../positive-definite-operator.md) $\alpha$ using the proved [spectral theorem](../../../../../../spectral-theorem.md). Its eigenvalues $\lambda_j$ are strictly positive, because $\langle\alpha e_j,e_j\rangle=\lambda_j>0$. Define $\beta e_j=\sqrt{\lambda_j}e_j$. It is a positive-definite [Hermitian operator](../../../../../../hermitian-operator.md) and $\beta^2=\alpha$, establishing existence of the [positive square root of an operator](../../../../../../positive-square-root-of-an-operator.md).

For uniqueness, let $B$ be any positive-definite Hermitian square root. The identity $B^2=\alpha$ implies $B\alpha=B^3=\alpha B$, so $B$ preserves each eigenspace $E_\lambda$ of $\alpha$. Its restriction to that space is Hermitian and positive-definite. Diagonalize that restriction by the same spectral theorem. Every resulting eigenvalue $\mu$ satisfies $\mu>0$ and $\mu^2=\lambda$, hence $\mu=\sqrt\lambda$. Therefore $B$ acts as $\sqrt\lambda I$ on the entire eigenspace, even when $\lambda$ is repeated. These eigenspaces span the space, so **the positive-definite Hermitian square root is unique**, with eigenvalues $\sqrt{\lambda_j}$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [11E](../../11e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
