<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $r=k-l$. Since $k$ and $l$ are even and $k\geq l+6$, one has $r\geq6$. The holomorphic [Eisenstein series](../../../../../../eisenstein-series.md) in the question is absolutely convergent and decomposes as

$$
G_r(\tau)
=2\zeta(r)\sum_{\gamma\in\Gamma_\infty\backslash\Gamma(1)}j(\gamma,\tau)^{-r},
$$

because every nonzero integer pair is a positive multiple of a primitive pair and the two signs contribute the factor two.

Absolute convergence, including that established in part (c) at $s=k-1$, permits [Rankin–Selberg unfolding](../../../../../../rankin-selberg-method.md). Unfolding the [Petersson inner product](../../../../../../petersson-inner-product.md) from the fundamental domain to the strip $0\leq x<1$, $y>0$, gives

$$
\langle f,gG_r\rangle
=2\zeta(r)\int_0^\infty\int_0^1
f(\tau)\overline{g(\tau)}y^{k-2}\,dx\,dy.
$$

The $x$-integral uses [orthogonality of complex exponentials](../../../../../../orthogonality-of-complex-exponentials.md) to retain equal Fourier indices:

$$
\int_0^1f(\tau)\overline{g(\tau)}\,dx
=\sum_{n\geq1}a_n\overline{b_n}e^{-4\pi ny}.
$$

Finally,

$$
\int_0^\infty e^{-4\pi ny}y^{k-2}\,dy
=\frac{\Gamma(k-1)}{(4\pi n)^{k-1}}.
$$

Substitution gives the [Rankin–Selberg unfolding identity for a holomorphic Eisenstein series](../../../../../../rankin-selberg-unfolding-identity-for-a-holomorphic-eisenstein-series.md)

$$
\boxed{\langle f,gG_{k-l}\rangle
=\frac{2\zeta(k-l)\Gamma(k-1)}{(4\pi)^{k-1}}L(f,g,k-1).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
