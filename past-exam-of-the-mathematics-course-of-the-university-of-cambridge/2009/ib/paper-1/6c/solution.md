<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

Subtract the exact solution from the [Jacobi method](../../../../../jacobi-method.md) to get $e_n=He_{n-1}$, hence $e_n=H^ne_0$. Convergence from every initial vector is equivalent to $H^n\to0$. If every [eigenvalue](../../../../../eigenvalue.md) has modulus below one, a [Jordan block](../../../../../jordan-block.md) $\lambda I+N$ has powers that are finite sums $\binom nk\lambda^{n-k}N^k$. The [polynomial](../../../../../polynomial-split.md) factor in $n$ is dominated by geometric decay; for $\lambda=0$, the block is nilpotent. Consequently $H^n\to0$.

Conversely, for a complex [eigenvector](../../../../../eigenvector.md) $v$ with [eigenvalue](../../../../../eigenvalue.md) $\lambda$, $H^nv=\lambda^nv$. Convergence for real errors also implies convergence for their complexification, so this tends to zero only if $|\lambda|<1$. Therefore **the iteration converges from every starting vector if and only if $\rho(H)<1$**, where $\rho$ is the [spectral radius](../../../../../spectral-radius.md).

For the specified [matrix](../../../../../matrix.md),

$$
H=\begin{pmatrix}0&0&\mu\\\mu/3&0&\mu/3\\\mu&0&0\end{pmatrix},\qquad \det(tI-H)=t(t^2-\mu^2).
$$

Its [eigenvalues](../../../../../eigenvalue.md) are $0,\mu,-\mu$, so $\rho(H)=|\mu|$. Hence **$-1<\mu<1$** is the convergence range. The original coefficient [matrix](../../../../../matrix.md) has determinant $12(1-\mu^2)$, so the endpoints also violate its assumed nonsingularity.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
