<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Condition on a [frailty random variable](../../../../../../frailty-random-variable.md) value $U=u$. Integrating the conditional [hazard function](../../../../../../hazard-function.md) gives $u e^{\beta z}H_0(t)$, so the conditional [survivor function](../../../../../../survival-function.md) is

$$
\Pr(T>t\mid U=u,z)=\exp\{-u e^{\beta z}H_0(t)\}.
$$

Average this conditional probability over the common frailty density $g$:

$$
\overline F^{(z)}(t)
=\int_0^\infty e^{-u e^{\beta z}H_0(t)}g(u)\,du.
$$

By definition the [Laplace transform](../../../../../../laplace-transform.md) of $g$ is $\widetilde g(s)=\int_0^\infty e^{-su}g(u)\,du$. Hence

$$
\boxed{\overline F^{(z)}(t)=\widetilde g\bigl(e^{\beta z}H_0(t)\bigr).}
$$

This averages [survivor functions](../../../../../../survival-function.md), not hazards. Differentiating its logarithm, when justified, gives

$$
\overline h^{(z)}(t)
=e^{\beta z}h_0(t)\frac{\int_0^\infty u e^{-u e^{\beta z}H_0(t)}g(u)\,du}
{\int_0^\infty e^{-u e^{\beta z}H_0(t)}g(u)\,du}
=e^{\beta z}h_0(t)\mathbb E[U\mid T>t,z].
$$

Thus the population [hazard function](../../../../../../hazard-function.md) uses the mean frailty among current survivors, explaining why a conditional [proportional hazards model](../../../../../../proportional-hazards-model.md) may cease to be proportional after frailty is integrated out.

## ↑ Ancestors (11)

1. [B](../b.md)
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
