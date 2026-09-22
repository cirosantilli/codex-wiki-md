<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

A [bounded operator](../../../../../continuous-linear-operator.md) on a complex [Hilbert space](../../../../../hilbert-space-split.md) is [self-adjoint](../../../../../self-adjoint-operator.md) when $T=T^*$, equivalently $\langle Tx,y\rangle=\langle x,Ty\rangle$. The [spectral theorem for compact self-adjoint operators](../../../../../spectral-theorem-for-compact-hermitian-operators.md) says its nonzero spectrum consists of real [eigenvalues](../../../../../eigenvalue.md) of finite multiplicity, with at most countably many and with accumulation possible only at zero. Their [eigenspaces](../../../../../eigenspace.md) are mutually orthogonal; their closed span is the [orthogonal complement](../../../../../orthogonal-complement.md) of the kernel. On that span the operator has the norm-convergent spectral action $Tx=\sum_j\lambda_j\langle x,e_j\rangle e_j$.

Take $H=\ell^2(\mathbb N)$ and $Te_n=e_n/n$. It is [self-adjoint](../../../../../self-adjoint-operator.md) and has infinite-dimensional range. Truncation to the first $N$ coordinates is a [finite-rank operator](../../../../../finite-rank-operator.md) and differs from $T$ in norm by $1/(N+1)$, so $T$ is compact.

The [resolvent set](../../../../../resolvent-set-of-an-operator.md) comprises those $\lambda$ for which $T-\lambda I$ has a bounded everywhere-defined inverse; its complement is the [spectrum](../../../../../spectrum-functional-analysis.md), and the [point spectrum](../../../../../point-spectrum.md) consists of [eigenvalues](../../../../../eigenvalue.md). In this example

$$
\boxed{\sigma_p(T)=\{1/n:n\ge1\},\quad
\sigma(T)=\{0\}\cup\{1/n:n\ge1\},\quad
\rho(T)=\mathbb C\setminus\sigma(T)}.
$$

For $\lambda$ outside the displayed closed set the inverse is diagonal with entries $(1/n-\lambda)^{-1}$ uniformly bounded, proving membership of the resolvent. Each $1/n$ has [eigenvector](../../../../../eigenvector.md) $e_n$. Zero is not an [eigenvalue](../../../../../eigenvalue.md), but $\|Te_n\|\to0$ prevents a bounded inverse; also $(1/n)_n\in\ell^2$ has no preimage since that would be the non-square-summable constant sequence. This justifies every asserted spectral case.

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
