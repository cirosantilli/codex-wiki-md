<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $K(X)=|k(X)|>0$ on a smooth interval, with $X=\epsilon x$. For the [WKB approximation for a slowly varying oscillator](../../../../../../wkb-approximation-for-a-slowly-varying-oscillator.md), write

$$
y=\exp\left[\epsilon^{-1}S_0(X)+S_1(X)+\cdots\right].
$$

Substitution into $\epsilon^2y_{XX}+K(X)^2y=0$ gives, at the first two orders,

$$
(S_0')^2+K^2=0,\qquad 2S_0'S_1'+S_0''=0.
$$

Thus $S_0'=\pm iK$ and $S_1'=-K'/(2K)$. The leading [WKB approximation](../../../../../../wkb-approximation.md) is

$$
\boxed{y(x)\sim\frac1{\sqrt{K(\epsilon x)}}\left[C_+\exp\left(i\int_{x_*}^xK(\epsilon s)ds\right)+C_-\exp\left(-i\int_{x_*}^xK(\epsilon s)ds\right)\right]}.
$$

The $K^{-1/2}$ [amplitude](../../../../../../wave-amplitude.md) is the transport correction accompanying the rapid [wave phase](../../../../../../phase-waves.md). Real solutions are equivalent real sine and cosine combinations.

For validity, $K$ must be smooth, nonzero and slowly varying compared with the local wavelength. In physical $x$ derivatives, sufficient local checks are $|K_x|/K^2\ll1$ and $|K_{xx}|/K^3\ll1$. Indeed each displayed branch has relative residual

$$
\frac{y''+K^2y}{K^2y}=\frac{3K_x^2}{4K^4}-\frac{K_{xx}}{2K^3}.
$$

Smooth positive $K(X)$ bounded away from zero has these properties on fixed slow intervals. At a zero of $k$ the [WKB approximation](../../../../../../wkb-approximation.md) fails and a [classical turning point](../../../../../../classical-turning-point.md) requires a different local analysis, often an [Airy turning-point connection formula](../../../../../../airy-turning-point-connection-formula.md). Rapid variations, coefficient singularities and excessively long accumulation of [wave phase](../../../../../../phase-waves.md) error also lie outside this leading approximation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
