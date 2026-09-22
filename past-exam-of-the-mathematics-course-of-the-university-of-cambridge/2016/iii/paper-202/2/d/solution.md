<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The reference [Brownian motion](../../../../../../brownian-motion-split.md) must start at $x$, and both laws must use the same stopped-path rule. Under the reference [probability measure](../../../../../../probability-measure.md) let $R_s=x+W_s$, let $\tau$ be its exit time from $(a,b)$, and put $T=t\wedge\tau$ and $c=(\delta-1)/2$. The **[Girsanov density for a stopped Bessel process](../../../../../../girsanov-density-for-a-stopped-bessel-process.md)**, as a functional of the stopped reference path, is

$$
\boxed{D(R)=\exp\left\{c\int_0^T\frac{dW_s}{R_s}-\frac{c^2}{2}\int_0^T\frac{ds}{R_s^2}\right\}.}
$$

Use the [predictable process](../../../../../../predictable-process.md) $\theta_s=cR_s^{-1}\mathbf1_{\{s\leq\tau\}}$, with any harmless choice at the endpoint. On $[0,t]$, $\int\theta_s^2ds\leq c^2t/a^2$. The [Novikov condition](../../../../../../novikov-s-condition.md) holds; under the density $D$, the [Girsanov theorem](../../../../../../girsanov-theorem.md) makes $\widetilde W_s=W_s-\int_0^s\theta_u du$ a [Brownian motion](../../../../../../brownian-motion-split.md). Before exit, $dR_s=cR_s^{-1}ds+d\widetilde W_s$, which is the required [stochastic differential equation](../../../../../../stochastic-differential-equation.md). The drift is a [locally Lipschitz function](../../../../../../locally-lipschitz-function.md) on $(0,\infty)$, so [pathwise uniqueness](../../../../../../pathwise-uniqueness.md) and [uniqueness in law](../../../../../../uniqueness-in-law.md) hold up to this exit time.

For a version involving just the endpoint and an ordinary integral, the [Itô formula](../../../../../../ito-s-lemma.md) for $\log R$ gives

$$
\int_0^T\frac{dW_s}{R_s}=\log\frac{R_T}{x}+\frac12\int_0^T\frac{ds}{R_s^2}.
$$

Thus

$$
\boxed{D(R)=\left(\frac{R_T}{x}\right)^{(\delta-1)/2}\exp\left\{-\frac{(\delta-1)(\delta-3)}8\int_0^T\frac{ds}{R_s^2}\right\}.}
$$

The stopped density is [measurable](../../../../../../measurability.md) from the stopped path, so it is also the [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) of the stopped-path laws. The stopping times in this formula are evaluated on the reference path, rather than taken from a different realization of $X$. A zero-start reference [Brownian motion](../../../../../../brownian-motion-split.md) would have a different deterministic initial value and could not dominate this law.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
