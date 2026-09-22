<h1 id="16b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Repeated differentiation of the [Gaussian function](../../../../../../gaussian-function.md) gives $D^ne^{-x^2}=P_n(x)e^{-x^2}$, where $P_0=1$ and $P_{n+1}=P_n'-2xP_n$. Induction shows $P_n$ has [degree of a polynomial](../../../../../../degree-of-a-polynomial.md) $n$ and leading coefficient $(-2)^n$: the differentiated term has lower degree, while multiplication by $-2x$ raises it by one. Thus the [Hermite polynomial](../../../../../../hermite-polynomial.md) $H_n=(-1)^nP_n$ has **degree $n$ and leading coefficient $2^n$**.

For $m<n$, apply [integration by parts](../../../../../../integration-by-parts.md) $n$ times to the Rodrigues expression:

$$
\int_{-\infty}^{\infty}H_nH_m e^{-x^2}\,dx=(-1)^n\int_{-\infty}^{\infty}H_m D^ne^{-x^2}\,dx=\int_{-\infty}^{\infty}H_m^{(n)}e^{-x^2}\,dx=0.
$$

All boundary terms vanish because each derivative of $e^{-x^2}$ is a [polynomial](../../../../../../polynomial-split.md) times that exponential, and such products tend to zero at either infinity. The same result for $m>n$ follows by symmetry of the [inner product](../../../../../../inner-product.md). The diagonal value is positive; indeed $H_n^{(n)}=2^nn!$ gives

$$
\boxed{(H_n,H_m)=2^nn!\sqrt\pi\,\delta_{nm}.}
$$

This proves the requested [orthogonality](../../../../../../orthogonal-vectors.md) as well as its normalization.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16B](../../16b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
