<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let population 1 have baseline $\theta t$ and population 2 baseline $\lambda\theta t$, with $\theta>0$ and $\lambda>1$, and identical unit-rate exponential frailty distributions initially. Their population [hazard functions](../../../../../../hazard-function.md) have ratio, for $t>0$,

$$
\boxed{R(t)=\frac{\overline h_2(t)}{\overline h_1(t)}=\lambda\frac{1+\theta t^2/2}{1+\lambda\theta t^2/2}.}
$$

At exactly $t=0$, both population hazards are zero, so their literal ratio is $0/0$ and is undefined. The intended initial comparison is the right-hand limit,

$$
\boxed{R(0+)=\lambda,\qquad \lim_{t\to\infty}R(t)=1.}
$$

With $z=\theta t^2/2$, $dR/dz=\lambda(1-\lambda)/(1+\lambda z)^2<0$, so the marginal [hazard ratio](../../../../../../hazard-ratio.md) decreases from $\lambda$ toward one. The faster-hazard population loses highly frail individuals sooner; its survivors become less frail than the first population's survivors.

Conditional on the same fixed frailty $u>0$, the individual [hazard ratio](../../../../../../hazard-ratio.md) is the constant $\lambda$. Marginalizing over frailty therefore destroys [proportional hazards](../../../../../../proportional-hazards-model.md), even though they hold at the individual level. A population-level [Cox proportional-hazards model](../../../../../../cox-proportional-hazards-model.md) that ignores frailty would impose an incorrect constant [hazard ratio](../../../../../../hazard-ratio.md) here. Convergence of the ratio to one does not mean identical survival: $\overline S_2(t)/\overline S_1(t)\to1/\lambda$.

## ↑ Ancestors (11)

1. [C](../c.md)
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
