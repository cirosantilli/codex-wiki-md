<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Bessel turning-point asymptotic](../../../../../../../bessel-turning-point-asymptotic.md) comes from a [cubic stationary endpoint](../../../../../../../cubic-stationary-endpoint.md), not an ordinary quadratic [stationary point](../../../../../../../stationary-point.md). Near $\vartheta=0$,

$$
\sin\vartheta-\vartheta=-\frac{\vartheta^3}{6}+O(\vartheta^5).
$$

Thus the contributing width is $\vartheta=O(n^{-1/3})$. On writing $\vartheta=(6/n)^{1/3}s$, the leading integral is

$$
J_n(n)\sim\frac1\pi\left(\frac6n\right)^{1/3}\int_0^\infty\cos(s^3)\,ds.
$$

The oscillatory integral is understood with a vanishing damping factor. Substitution $u=s^3$ and the [Gamma function](../../../../../../../gamma-function.md) Fourier integral give

$$
\int_0^\infty\cos(s^3)\,ds=\frac13\Gamma(1/3)\cos(\pi/6).
$$

Therefore

$$
\boxed{J_n(n)\sim\frac{6^{1/3}\Gamma(1/3)}{2\sqrt3\,\pi}\,n^{-1/3}
=\frac{2^{1/3}}{3^{2/3}\Gamma(2/3)}\,n^{-1/3}}.
$$

The equality uses the [Gamma reflection formula](../../../../../../../gamma-reflection-formula.md). Contributions away from the degenerate endpoint are smaller. The $n^{-1/3}$ scale explains why the preceding $n^{-1/2}$ formula cannot be extended directly to zero angle.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 74](../../../../paper-74-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
