<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\omega_n=(n-\tfrac12)\pi$. The deterministic derivative is $g_n'=-\omega_nh_n$, and $g_n(1)=0$, while $W_0=0$. The [Itô product rule](../../../../../../ito-product-rule.md) with a deterministic smooth function gives

$$
\xi_n=g_n(1)W_1-g_n(0)W_0-\int_0^1g_n'(t)W_t\,dt
=\boxed{\omega_n\int_0^1h_n(t)W_t\,dt.}
$$

Almost every Brownian path is continuous, hence belongs to $L^2[0,1]$. Its Fourier coefficient in the given [orthonormal basis](../../../../../../orthonormal-basis.md) $(h_n)$ is therefore $\xi_n/\omega_n$. The [Parseval identity for a Hilbertian basis](../../../../../../parseval-identity-for-a-hilbertian-basis.md) gives, pathwise on a probability-one event,

$$
\boxed{\int_0^1W_t^2\,dt=\sum_{n=1}^\infty\frac{\xi_n^2}{(n-\tfrac12)^2\pi^2}.}
$$

This is the squared-norm consequence of the [Brownian half-integer sine expansion](../../../../../../brownian-half-integer-sine-expansion.md); completeness, rather than pointwise convergence of a Fourier series, is all that is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
