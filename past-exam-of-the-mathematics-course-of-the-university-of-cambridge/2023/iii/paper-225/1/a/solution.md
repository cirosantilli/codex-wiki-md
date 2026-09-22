<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Karhunen–Loève expansion](../../../../../../karhunen-loeve-expansion.md) has the following Hilbert-space form. Let $X$ be a square-integrable [Random element of a Hilbert space](../../../../../../hilbert-space-valued-random-variable.md) $H$, with mean $\mu$ and [covariance operator](../../../../../../covariance-operator.md) $C$. There are nonnegative [eigenvalues](../../../../../../eigenvalue.md) $\lambda_1\geq\lambda_2\geq\cdots$ and orthonormal [eigenvectors](../../../../../../eigenvector.md) $\phi_k$ spanning the closure of the range of $C$ such that

$$
C\phi_k=\lambda_k\phi_k,
\qquad
X=\mu+\sum_{k\geq1}\xi_k\phi_k
$$

in $L^2(\Omega;H)$. The [functional principal component scores](../../../../../../functional-principal-component-score.md)

$$
\xi_k=\langle X-\mu,\phi_k\rangle
$$

satisfy

$$
\mathbb E\xi_k=0,
\qquad
\mathbb E[\xi_j\xi_k]=\lambda_k\mathbf1_{\{j=k\}}.
$$

If $X$ is a [Gaussian random element](../../../../../../gaussian-random-element.md), the scores are independent normal random variables.

For the proof, $C$ is positive, self-adjoint, and [trace-class](../../../../../../trace-class-operator.md), with

$$
\operatorname{tr}C=\mathbb E\lVert X-\mu\rVert^2<\infty.
$$

It is therefore [compact](../../../../../../compact-operator-split.md), so the [spectral theorem for compact Hermitian operators](../../../../../../spectral-theorem-for-compact-hermitian-operators.md) supplies the eigenpairs. Their score covariance is

$$
\mathbb E[\xi_j\xi_k]
=\langle C\phi_j,\phi_k\rangle
=\lambda_j\langle\phi_j,\phi_k\rangle.
$$

For the residual $R_m=X-\mu-\sum_{k=1}^m\xi_k\phi_k$, [Parseval identity](../../../../../../parseval-identity.md) and the trace formula give

$$
\mathbb E\lVert R_m\rVert^2
=\operatorname{tr}C-\sum_{k=1}^m\lambda_k
=\sum_{k>m}\lambda_k\longrightarrow0.
$$

The centered variable's projection onto $\ker C$ has zero second moment and is therefore zero almost surely, which completes the mean-square expansion. When $C$ has a continuous covariance kernel, [Mercer's theorem](../../../../../../mercer-s-theorem.md) additionally expands that kernel as $c(s,t)=\sum_k\lambda_k\phi_k(s)\phi_k(t)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
