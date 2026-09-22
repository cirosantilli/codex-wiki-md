<h1 id="18f/solution">Solution</h1>

↑ **Parent:** [18F](../18f.md)

Let $x_*=A^{-1}b$ and $e^{(k)}=x^{(k)}-x_*$. The [Richardson iteration](../../../../../richardson-iteration.md) gives

$$
e^{(k+1)}=(I-\tau A)e^{(k)},\qquad e^{(k)}=(I-\tau A)^ke^{(0)}.
$$

By the [spectral theorem](../../../../../spectral-theorem.md), a real symmetric positive definite [matrix](../../../../../matrix.md) has an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) with positive [eigenvalues](../../../../../eigenvalue.md) $\lambda_1,\ldots,\lambda_n$. The error in the $i$th [eigenvector](../../../../../eigenvector.md) direction is multiplied by $(1-\tau\lambda_i)^k$. Thus convergence for every initial vector occurs exactly when $|1-\tau\lambda_i|<1$ for every $i$, or $0<\tau\lambda_i<2$. Since $\rho(A)=\lambda_{\max}$,

$$
\boxed{0<\tau<\frac2{\rho(A)}.}
$$

Necessity also follows from an initial error in an offending [eigenvector](../../../../../eigenvector.md) direction. At $\tau=0$ it remains unchanged; at $\tau=2/\rho(A)$ the largest-eigenvalue error alternates sign; outside the interval some error does not decay. Hence neither endpoint can be included.

## ↑ Ancestors (10)

1. [18F](../18f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
