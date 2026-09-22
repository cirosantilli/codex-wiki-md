<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a continuous [survival distribution](../../../../../../survival-distribution.md), $S(t)=e^{-H(t)}$, $h(t)=H'(t)$ and $f(t)=h(t)S(t)$. Applying these identities gives the [Weibull distribution](../../../../../../weibull-distribution.md)

$$
\boxed{S(t)=e^{-(\lambda t)^p},\qquad
h(t)=p\lambda^pt^{p-1},\qquad
f(t)=p\lambda^pt^{p-1}e^{-(\lambda t)^p},\quad t>0.}
$$

The [survivor function](../../../../../../survival-function.md) has value one at zero; the [hazard](../../../../../../hazard-function.md) may diverge there when $p<1$, which does not invalidate the distribution.

For common shape $p$, the [hazard ratio](../../../../../../hazard-ratio.md) is $h_2(t)/h_1(t)=(\lambda_2/\lambda_1)^p$, independent of time. Thus the two distributions lie in the same [proportional hazards family](../../../../../../proportional-hazards-family.md). They also satisfy

$$
S_2(t)=S_1\left(\frac{\lambda_2}{\lambda_1}t\right),\qquad
T_2\overset d=\frac{\lambda_1}{\lambda_2}T_1.
$$

Hence **the time multiplier is $\lambda_1/\lambda_2$ and the [hazard](../../../../../../hazard-function.md) multiplier is $(\lambda_2/\lambda_1)^p$**, establishing the common [accelerated life family](../../../../../../accelerated-life-family.md) as well. Here $\lambda$ is reciprocal scale, not the ordinary time-scale parameter.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
