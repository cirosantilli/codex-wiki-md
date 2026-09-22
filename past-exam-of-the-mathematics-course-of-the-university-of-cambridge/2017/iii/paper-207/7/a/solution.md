<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [frailty model](../../../../../../frailty-model.md) represents unobserved heterogeneity using a nonnegative [frailty random variable](../../../../../../frailty-random-variable.md) $U$ that multiplies an individual's [baseline hazard](../../../../../../baseline-hazard.md). With $H_0(t)=\int_0^th_0(s)\,ds$, the individual and population [survivor functions](../../../../../../survival-function.md) are

$$
S(t\mid U=u)=e^{-uH_0(t)},\qquad \overline S(t)=\int_0^\infty e^{-uH_0(t)}g(u)\,du.
$$

Thus the population [survivor function](../../../../../../survival-function.md) is the [Laplace transform](../../../../../../laplace-transform.md) of the frailty distribution at $H_0(t)$; at points where differentiation is justified, $\overline h(t)=h_0(t)\mathbb E[U\mid T>t]$. The last identity follows by differentiating the integral and dividing $-\overline S'$ by $\overline S$.

Here $g(u)=e^{-u}$ for $u\geq0$, $\theta>0$, and $H_0(t)=\theta t^2/2$. Direct integration gives

$$
\boxed{\overline S(t)=\frac1{1+\theta t^2/2},\qquad \overline h(t)=\frac{\theta t}{1+\theta t^2/2}.}
$$

This is [population hazard under exponential frailty](../../../../../../population-hazard-under-exponential-frailty.md). For every fixed $u>0$ the individual [hazard function](../../../../../../hazard-function.md) $u\theta t$ increases linearly. In contrast,

$$
\overline h'(t)=\frac{\theta(1-\theta t^2/2)}{(1+\theta t^2/2)^2},
$$

so the population hazard increases up to $t=\sqrt{2/\theta}$, then decreases, tending to zero like $2/t$. More vulnerable individuals leave the [risk set](../../../../../../risk-set.md) earlier, leaving survivors with smaller frailties. This population decline is selection, not a decline in any fixed individual's hazard. If $\theta=0$, survival is identically one and both hazards vanish; the positive-rate comparison is then inapplicable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
