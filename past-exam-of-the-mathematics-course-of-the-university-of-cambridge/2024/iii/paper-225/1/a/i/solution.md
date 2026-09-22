<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

This is the [Brownian covariance kernel](../../../../../../../brownian-covariance-kernel.md), so its integral operator is a [covariance operator](../../../../../../../covariance-operator.md). To obtain its [eigendecomposition](../../../../../../../spectral-decomposition.md), suppose $Uf=\lambda f$ with $\lambda\ne0$. Splitting the integral at $s$ gives

$$
\lambda f(s)=\int_0^s t f(t)dt+s\int_s^1f(t)dt.
$$

Differentiation yields $\lambda f'(s)=\int_s^1f(t)dt$ and $\lambda f''(s)=-f(s)$, with boundary conditions $f(0)=0$ and $f'(1)=0$. Hence the normalized eigenpairs are

$$
\phi_k(t)=\sqrt2\sin\!\left((k-\tfrac12)\pi t\right),
\qquad
\lambda_k=\frac1{(k-\tfrac12)^2\pi^2},
\qquad k\geq1.
$$

The eigenvalues are positive and summable, consistently with positivity and the [trace-class operator](../../../../../../../trace-class-operator.md) property of a covariance operator.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 225](../../../../paper-225-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
