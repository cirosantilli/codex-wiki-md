<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply part [a](../a.md) with $\alpha=r$. For $\tau>0$, the [transition density](../../../../transition-density.md) is the [normal distribution](../../../../normal-distribution.md) with mean $m=Se^{r\tau}$ and positive [variance](../../../../variance-split.md) $v=\sigma^2(e^{2r\tau}-1)/(2r)$. Integrating the [financial payoff](../../../../contingent-claim-payoff.md) against this [probability density function](../../../../probability-density-function.md) gives

$$
\boxed{V(S,t)=\frac{e^{-r\tau}}{\sqrt{2\pi v}}
\int_{-\infty}^{\infty}P_{\mathrm o}(x)
\exp\!\left[-\frac{(x-Se^{r\tau})^2}{2v}\right]dx,\qquad
v=\frac{\sigma^2}{2r}(e^{2r\tau}-1).}
$$

Thus $d_*=(x-Se^{r\tau})/\sqrt v$, as required. The [variance](../../../../variance-split.md) is positive even if $r<0$, because numerator and denominator have the same sign. For $r=0$, replace $m$ by $S$ and $v$ by $\sigma^2\tau$; at expiry use the terminal value directly. The [integral](../../../../integral-split.md) presumes an integrable [financial payoff](../../../../contingent-claim-payoff.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
