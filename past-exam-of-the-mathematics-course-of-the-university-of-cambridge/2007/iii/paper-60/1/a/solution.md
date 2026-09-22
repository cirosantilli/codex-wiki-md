<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the real [vector space](../../../../../../vector-space-split.md) of [Hermitian matrices](../../../../../../hermitian-operator.md) and its [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md) $\langle A,B\rangle=\operatorname{Tr}(AB)$. A Hermitian $N$-by-$N$ [matrix](../../../../../../matrix.md) has $N$ real diagonal entries and two real parameters for each off-diagonal pair, hence real dimension $N+2\binom N2=N^2$. Imposing zero [trace](../../../../../../matrix-trace.md) removes one real dimension. Each supplied [generalized Pauli matrix](../../../../../../generalized-pauli-matrix.md) is Hermitian and traceless, and there are $N(N-1)$ off-diagonal matrices and $N-1$ diagonal matrices, totaling $N^2-1$.

Their assumed [orthonormality](../../../../../../orthonormal-set.md) makes them linearly independent. Since this equals the dimension of the traceless space, **they are an orthonormal basis of the traceless Hermitian matrices**. To extend the family, the required additional generator is $\sigma_0=I/\sqrt N$, which is implicit in the indexing of the question. It has unit [Hilbert-Schmidt norm](../../../../../../hilbert-schmidt-norm.md) and is orthogonal to every traceless generator, so the extended family is an [orthonormal basis](../../../../../../orthonormal-basis.md) of all Hermitian matrices.

For a [density operator](../../../../../../density-matrix.md) $\rho$, cyclicity of the [trace](../../../../../../matrix-trace.md) gives

$$
s_k^*=\operatorname{Tr}((\rho\sigma_k)^\dagger)=\operatorname{Tr}(\sigma_k\rho)=\operatorname{Tr}(\rho\sigma_k)=s_k.
$$

Thus **$s\in\mathbb R^{N^2-1}$**. Since $\operatorname{Tr}\rho=1$, the resulting [Generalized Bloch representation](../../../../../../generalized-bloch-representation.md) is

$$
\rho=\frac IN+\sum_{k=1}^{N^2-1}s_k\sigma_k.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
