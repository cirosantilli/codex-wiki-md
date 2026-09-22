<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\sigma^2>0$, a [gamma distribution](../../../../../../gamma-distribution.md) with unit mean and [variance](../../../../../../variance-split.md) $\sigma^2$ has shape and rate $\psi=1/\sigma^2$. Substituting its [Laplace transform](../../../../../../laplace-transform.md) into the preceding result gives

$$
\overline F^{(z)}(t)
=\left(1+\sigma^2e^{\beta z}H_0(t)\right)^{-1/\sigma^2}.
$$

Its negative logarithmic derivative is the population [hazard function](../../../../../../hazard-function.md):

$$
\overline h^{(z)}(t)
=\frac{e^{\beta z}h_0(t)}{1+\sigma^2 e^{\beta z}H_0(t)}.
$$

Consequently, at times with $h_0(t)>0$, the [gamma frailty hazard ratio](../../../../../../gamma-frailty-hazard-ratio.md) is

$$
\boxed{r(t)=e^\beta\frac{1+\sigma^2H_0(t)}{1+\sigma^2 e^\beta H_0(t)}.}
$$

At a time when both hazards vanish this formula is a continuous extension; the literal ratio $0/0$ is undefined.

Write $a=e^\beta>0$ and $x=\sigma^2H_0(t)\geq0$. Two useful identities are

$$
r-1=\frac{a-1}{1+ax},\qquad
\frac{dr}{dx}=\frac{a(1-a)}{(1+ax)^2}.
$$

For small cumulative exposure $x$, $r=a\{1+(1-a)x+O(x^2)\}$, so it starts at the conditional [hazard ratio](../../../../../../hazard-ratio.md) $e^\beta$. If $\beta>0$, it decreases towards one; if $\beta<0$, it increases towards one; and if $\beta=0$, it equals one throughout. It stays between $e^\beta$ and one and never crosses one.

For fixed $\sigma^2>0$, **the late-time limit is one provided $H_0(t)\to\infty$**. If instead the [integrated hazard](../../../../../../cumulative-hazard-function.md) tends to a finite value $K$, the limiting [hazard ratio](../../../../../../hazard-ratio.md) is $a(1+\sigma^2K)/(1+a\sigma^2K)$, which need not be one. Elapsed time alone does not imply unbounded exposure.

For small $\sigma^2$ at a fixed time, $r\to e^\beta$. At $\sigma^2=0$ the frailty degenerates to $U=1$, giving an ordinary [proportional hazards model](../../../../../../proportional-hazards-model.md). For large $\sigma^2$ at a fixed time with $H_0(t)>0$, $r\to1$; at time zero, however, it remains $e^\beta$. Thus that variance limit is not uniform near zero. Larger heterogeneity accelerates the movement of the population [hazard ratio](../../../../../../hazard-ratio.md) towards one. The mechanism is [survival selection](../../../../../../survival-selection-in-a-heterogeneous-population.md): frailer individuals leave the population sooner, particularly in the higher-hazard group, while each individual's conditional multiplier remains fixed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
