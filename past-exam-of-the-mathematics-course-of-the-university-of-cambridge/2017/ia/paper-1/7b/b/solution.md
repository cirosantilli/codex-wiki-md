<h1 id="7b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A real [skew-symmetric matrix](../../../../../../skew-symmetric-matrix.md) satisfies $A^\dagger=A^T=-A$, so it is a [skew-Hermitian matrix](../../../../../../skew-hermitian-matrix.md). If $Ax=\lambda x$, then

$$
\lambda\,x^\dagger x=x^\dagger Ax.
$$

Taking the [complex conjugate](../../../../../../complex-conjugate.md) and using $A^\dagger=-A$ shows that this scalar is the negative of its conjugate. Hence

$$
\boxed{\lambda^*=-\lambda},
$$

so every eigenvalue is purely imaginary or zero.

If $Ax=\lambda x$ and $Ay=\mu y$, then

$$
\lambda^*x^\dagger y=(Ax)^\dagger y=x^\dagger A^\dagger y=-\mu x^\dagger y.
$$

Since $\lambda^*=-\lambda$, this becomes $(\mu-\lambda)x^\dagger y=0$. Distinct eigenvalues therefore have orthogonal eigenvectors:

$$
\boxed{\lambda\ne\mu\implies x^\dagger y=0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
