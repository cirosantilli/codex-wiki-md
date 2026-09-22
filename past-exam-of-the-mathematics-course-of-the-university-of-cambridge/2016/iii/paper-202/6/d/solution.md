<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Work before the first zero of $Z$, with $Z_0=z>0$. For the [Bessel process](../../../../../../bessel-process.md) equation, the [Itô formula](../../../../../../ito-s-lemma.md) applied to $x^r$ gives

$$
\boxed{dW_t=rZ_t^{r-1}dB_t+\frac{r(\delta+r-2)}2Z_t^{r-2}dt,\qquad W_0=z^r.}
$$

Its [quadratic variation](../../../../../../quadratic-variation.md) is

$$
C_t=[W]_t=r^2\int_0^tZ_u^{2r-2}du.
$$

This clock is strictly increasing on the positive-state interval. For $s$ before its terminal clock value, let $Y_s=W_{\sigma_s}$ and let $\beta_s=(\int_0^\cdot rZ_u^{r-1}dB_u)_{\sigma_s}$. The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) makes $\beta$ a [Brownian motion](../../../../../../brownian-motion-split.md) there. Since $d\sigma_s=ds/(r^2Z_{\sigma_s}^{2r-2})$, the drift changes to

$$
\frac{r(\delta+r-2)}2\frac{Z_{\sigma_s}^{r-2}}{r^2Z_{\sigma_s}^{2r-2}}=\frac{\delta+r-2}{2rY_s}.
$$

Consequently the **[Power time change of a Bessel process](../../../../../../power-time-change-of-a-bessel-process.md)** gives

$$
\boxed{dY_s=d\beta_s+\frac{\delta'-1}{2Y_s}ds,\qquad\delta'=2+\frac{\delta-2}{r}.}
$$

The initial value is $z^r$, and this equation identifies a [Bessel process](../../../../../../bessel-process.md) of dimension $\delta'$ until its first zero. Localize both equations on compact subintervals of $(0,\infty)$ to justify the inverse and all [stochastic integrals](../../../../../../stochastic-integral.md) for arbitrary $r>0$.

For completeness, the inverse-clock lifetime really is the positive [Bessel process](../../../../../../bessel-process.md) lifetime: the map $z\mapsto z^r$ is a homeomorphism of $(0,\infty)$, and exits from nested compact intervals correspond under the clock. There is no finite explosion at infinity for a positive [Bessel process](../../../../../../bessel-process.md), since the [Itô formula](../../../../../../ito-s-lemma.md) for $Y^2$ gives $d(Y^2)=2Y\,d\beta+\delta'ds$; stopping at zero or level $R$ yields a probability of hitting $R$ before a fixed $T$ bounded by $(Y_0^2+\max(\delta',0)T)/R^2$. If the transformed lifetime were finite while $Y$ stayed in a compact positive interval, the inverse clock and the original solution could both be continued. Thus a finite lifetime is approach to zero. For $\delta<2$, also $\delta'<2$ and the positive-state [Bessel process](../../../../../../bessel-process.md) hits zero; for $\delta\geq2$ the transformed lifetime is infinite. No continuation through zero is needed.

If the initial value is already zero, the interval before its first zero is empty; the positive-state argument concerns starts $z>0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
