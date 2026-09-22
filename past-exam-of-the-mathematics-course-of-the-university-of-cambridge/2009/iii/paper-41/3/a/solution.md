<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [proportional hazards family](../../../../../../proportional-hazards-family.md) has a common [baseline hazard](../../../../../../baseline-hazard.md) $h_0$ and positive constants $a_z$ such that $h_z(t)=a_z h_0(t)$. Thus its [hazard ratios](../../../../../../hazard-ratio.md) are constant in time, and its [survivor functions](../../../../../../survival-function.md) satisfy $S_z(t)=S_0(t)^{a_z}$. An [accelerated life family](../../../../../../accelerated-life-family.md) instead has positive constants $c_z$ such that $T_z$ has the distribution of $c_zT_0$. Equivalently, $S_z(t)=S_0(t/c_z)$: all time [quantiles](../../../../../../quantile-function.md) are multiplied by the same factor. These two properties are generally different.

Integrating the printed [Weibull distribution](../../../../../../weibull-distribution.md) density, or differentiating the following expression and checking its initial value, gives

$$
S_{p,\lambda}(t)=\exp[-(\lambda t)^p],\qquad
H_{p,\lambda}(t)=(\lambda t)^p,\qquad
h_{p,\lambda}(t)=p\lambda^p t^{p-1}.
$$

Here $\lambda$ is an inverse-time parameter: the coefficient of $t^p$ in the [cumulative hazard](../../../../../../cumulative-hazard-function.md) is $\lambda^p$, not $\lambda$. This matters when comparing different parameterizations of a [Weibull distribution](../../../../../../weibull-distribution.md).

With common shape $p$, the [hazard ratio](../../../../../../hazard-ratio.md) is

$$
\boxed{\frac{h_{p,\lambda_1}(t)}{h_{p,\lambda_2}(t)}
=\left(\frac{\lambda_1}{\lambda_2}\right)^p.}
$$

It does not depend on $t$, proving membership in one [proportional hazards family](../../../../../../proportional-hazards-family.md). For the other property,

$$
S_{p,\lambda_1}(t)=S_{p,\lambda_2}\left(\frac{\lambda_1}{\lambda_2}t\right),
\qquad
\boxed{T_1\ \overset{d}{=}\ \frac{\lambda_2}{\lambda_1}T_2.}
$$

Consequently they also belong to one [accelerated life family](../../../../../../accelerated-life-family.md). A larger inverse-time parameter gives shorter survival times and larger hazards, consistently in both descriptions. This is the common-shape case of [Weibull accelerated-life and proportional-hazards families](../../../../../../weibull-accelerated-life-and-proportional-hazards-families.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
