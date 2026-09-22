<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The printed pathwise conclusion is false without specifying the initial value.** We first prove exactly what the hypotheses do imply, by [stationary drift saturation](../../../../../../stationary-drift-saturation.md).

Stationarity gives $\mathbb E Z_s^2=1$. The [Itô formula](../../../../../../ito-s-lemma.md) yields

$$
d(Z_s^2)=2\sqrt{2\lambda}Z_s\,dW_s+(2Z_sg_s+2\lambda)ds.
$$

The [stochastic integral](../../../../../../stochastic-integral.md) is a true [square-integrable](../../../../../../square-integrable-function.md) [martingale](../../../../../../martingale-split.md) on every finite horizon, since $\mathbb E\int_0^tZ_s^2ds=t$. Also $\mathbb E|Z_sg_s|\le\lambda$ by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Taking expectations therefore gives

$$
0=2\int_0^t\bigl(\mathbb E[Z_sg_s]+\lambda\bigr)ds.
$$

Every integrand is nonnegative, so $\mathbb E[Z_sg_s]=-\lambda$ for almost every $s$. For those times,

$$
\mathbb E(g_s+\lambda Z_s)^2
=\mathbb Eg_s^2+2\lambda\mathbb E(Z_sg_s)+\lambda^2\mathbb EZ_s^2\le0.
$$

It follows that $g_s=-\lambda Z_s$ for almost every time and outcome. Equality of these integrable drift terms gives the exact solution

$$
Z_t=e^{-\lambda t}Z_0+\sqrt{2\lambda}\int_0^te^{-\lambda(t-s)}dW_s,
\qquad
\boxed{Z_t-Y_t=e^{-\lambda t}(Z_0-B_1).}
$$

Thus $Z$ solves the same equation, but stationarity has not identified its initial random variable with $B_1$.

For an explicit counterexample, take

$$
Z_0=-B_1,\qquad
Z_t=-e^{-\lambda t}B_1+\sqrt{2\lambda}\int_0^te^{-\lambda(t-s)}dW_s,
\qquad g_t=-\lambda Z_t.
$$

This is adapted to $\mathcal G_t$. Its independent normal initial value and Brownian noise make it a centered stationary [Gaussian process](../../../../../../gaussian-process.md) with [covariance](../../../../../../covariance.md) $e^{-\lambda|t-s|}$, exactly as for $Y$. Hence $\mathbb EZ_0^2=1$ and $\mathbb Eg_t^2=\lambda^2$, satisfying every printed hypothesis. Nevertheless $Z_t-Y_t=-2e^{-\lambda t}B_1$, which is nonzero almost surely for every finite $t$.

The corrected result is **indistinguishability if one adds $Z_0=Y_0$ almost surely**. Without that addition, there is equality in law of the stationary Ornstein-Uhlenbeck processes, not necessarily equality of their coupled paths. To see that the initial law is forced, independence of [Brownian increments](../../../../../../brownian-increment.md) from $\mathcal G_0$ and stationarity give, for its [characteristic function](../../../../../../characteristic-function.md) $\varphi$,

$$
\varphi(u)=\varphi(e^{-\lambda t}u)\exp\!\left[-\tfrac12(1-e^{-2\lambda t})u^2\right].
$$

Letting $t\to\infty$ proves $\varphi(u)=e^{-u^2/2}$. This is the distinction captured by [same-noise stationary Ornstein-Uhlenbeck processes](../../../../../../same-noise-stationary-ornstein-uhlenbeck-processes.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
