<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $f(n)=3^{\omega(n)}$, where $\omega$ is the [prime omega function](../../../../../../prime-omega-function.md). If $p^a\Vert n$, its contribution to the [Dirichlet convolution](../../../../../../dirichlet-convolution.md) $(f*\Lambda)(n)$ is

$$
\sum_{j=1}^af(n/p^j)\log p=f(n)(a-1+1/3)\log p.
$$

Since $3(a-1+1/3)\geq a$, summing over the [prime factors](../../../../../../prime-factor.md) proves the [log-weighted convolution bound for three to the prime omega](../../../../../../log-weighted-convolution-bound-for-three-to-the-prime-omega.md), $f(n)\log n\leq3(f*\Lambda)(n)$. On $\sqrt D\leq n\leq D$, $\log n\geq\tfrac12\log D$, hence

$$
\sum_{\sqrt D\leq n\leq D}f(n)
\leq\frac6{\log D}\sum_{n\leq D}(f*\Lambda)(n)
=\frac6{\log D}\sum_{m\leq D}f(m)\psi(D/m).
$$

This is the required inequality. The standard [Chebyshev estimate](../../../../../../chebyshev-estimate.md) $\psi(t)\ll t$ bounds its right side by $D(\log D)^{-1}\sum_{m\leq D}f(m)/m$. To bound the latter [sum](../../../../../../sum.md), use [multiplicativity](../../../../../../multiplicativity-of-an-arithmetic-function.md) and extend to all numbers with [prime factors](../../../../../../prime-factor.md) at most $D$:

$$
\sum_{m\leq D}\frac{f(m)}m\leq\prod_{p\leq D}\left(1+\frac3{p-1}\right).
$$

The [Mertens second theorem](../../../../../../mertens-second-theorem.md) states $\sum_{p\leq D}1/p=\log\log D+O(1)$. Taking [logarithms](../../../../../../logarithm.md) of the product, with a summable $O(p^{-2})$ remainder, gives $3\log\log D+O(1)$. Therefore the product is $O(\log^3D)$, proving the [summatory bound for three to the prime omega](../../../../../../summatory-bound-for-three-to-the-prime-omega.md) in the required range:

$$
\boxed{\sum_{\sqrt D\leq n\leq D}3^{\omega(n)}\ll D\log^2D.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
