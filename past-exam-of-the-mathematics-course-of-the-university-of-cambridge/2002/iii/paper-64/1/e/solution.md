<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The relevant boundary here is the [upper critical dimension](../../../../../../upper-critical-dimension.md): above it the critical interactions become negligible at long distances and the ordinary [mean-field critical exponents](../../../../../../mean-field-critical-exponent.md) apply; at it there can be logarithmic corrections. This differs from the [lower critical dimension](../../../../../../lower-critical-dimension.md), below which a particular kind of ordering may fail to exist.

Normalize the coefficient of $(\nabla\phi)^2$ in the [Landau-Ginzburg theory](../../../../../../landau-ginzburg-theory.md). Under a change of length scale $x=bx'$, its invariance gives the [engineering dimension](../../../../../../engineering-dimension.md) $x_\phi=(d-2)/2$. The quartic interaction then scales as

$$
u'=b^{d-4x_\phi}u=b^{4-d}u.
$$

It is a [relevant operator](../../../../../../relevant-operator.md) below four dimensions and an [irrelevant operator](../../../../../../irrelevant-operator.md) above four. Thus **the ordinary scalar transition has upper critical dimension $d_c=4$**. At a [tricritical point](../../../../../../tricritical-point.md), where the quartic interaction is tuned away, the sextic coupling scales as $v'=b^{6-2d}v$, giving **the tricritical upper critical dimension $d_c=3$**. This is the [upper critical dimension of an even scalar interaction](../../../../../../upper-critical-dimension-of-an-even-scalar-interaction.md) applied to powers four and six.

The [Ginzburg criterion](../../../../../../ginzburg-criterion.md) makes the reason for failure of the [Landau approximation](../../../../../../landau-approximation.md) quantitative. In the ordered quartic theory, $M^2=|r|/u$, $V''(M)=2|r|$ and $\xi^2=K/(2|r|)$. The fluctuation of the [order parameter](../../../../../../order-parameter.md) averaged over a [correlation volume](../../../../../../correlation-volume.md) has the scale

$$
\left\langle(\delta\phi)^2\right\rangle_{\xi}
\asymp k_BT\int_{|q|\lesssim\xi^{-1}}\frac{d^dq}{(2\pi)^d}
\frac1{Kq^2+2|r|}
\asymp\frac{k_BT}{K}\xi^{2-d}.
$$

Compared with the squared mean [order parameter](../../../../../../order-parameter.md), the [Ginzburg criterion](../../../../../../ginzburg-criterion.md) therefore gives

$$
\frac{\langle(\delta\phi)^2\rangle_{\xi}}{M^2}
\asymp\frac{k_BTu}{K^2}\xi^{4-d}.
$$

For $d<4$ this ratio grows without bound as the [correlation length](../../../../../../correlation-length.md) diverges. The assumption that fluctuations are small relative to the ordered value fails arbitrarily near the transition, and the interacting [renormalization-group fixed point](../../../../../../renormalization-group-fixed-point.md) determines the [critical exponents](../../../../../../critical-exponent.md). For $d>4$ the ratio tends to zero. At $d=4$ scale counting is marginal, and the running quartic coupling produces logarithms.

Similarly, at the [tricritical point](../../../../../../tricritical-point.md) $M^2\asymp\sqrt{K/v}\,\xi^{-1}$, so the [multicritical Ginzburg ratio](../../../../../../multicritical-ginzburg-ratio.md) scales as $(k_BT\sqrt v/K^{3/2})\xi^{3-d}$. The [Landau-Ginzburg theory](../../../../../../landau-ginzburg-theory.md) remains a useful effective description below its [upper critical dimension](../../../../../../upper-critical-dimension.md); it is its fluctuation-free exponent calculation that fails, not the possibility of including fluctuations in the theory.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
