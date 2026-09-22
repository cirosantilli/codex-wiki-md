<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [unit-root autoregressive process](../../../../../../unit-root-autoregressive-process.md) retains shocks permanently, whereas a [causal time series](../../../../../../causal-time-series.md) with $|\phi|<1$ reverts towards its mean. Testing the unit root determines whether stationary autoregressive analysis is appropriate or [differencing](../../../../../../differencing.md) is needed. For the model without an intercept or trend, use the [Dickey–Fuller test](../../../../../../dickey-fuller-test.md) against the lower-sided alternative $\phi<1$ near the null. Put

$$
\widehat\phi=\frac{\sum_{t=2}^nX_{t-1}X_t}{\sum_{t=2}^nX_{t-1}^2},\qquad
\widehat\sigma^2=\frac1{n-2}\sum_{t=2}^n(X_t-\widehat\phi X_{t-1})^2,
\qquad T_n=\frac{(\widehat\phi-1)\sqrt{\sum_{t=2}^nX_{t-1}^2}}{\widehat\sigma}.
$$

This is the ordinary regression statistic for a zero coefficient when $\Delta X_t$ is regressed on $X_{t-1}$, but its null [probability distribution](../../../../../../probability-distribution.md) is not the usual Student law. Under the standard unit-root initialization $X_1=o_P(\sqrt n)$ and innovations independent of the starting value,

$$
T_n\Rightarrow D=\frac{\int_0^1 W(u)\,dW(u)}{\sqrt{\int_0^1W(u)^2\,du}}
=\frac{W(1)^2-1}{2\sqrt{\int_0^1W(u)^2\,du}},
$$

where $W$ is standard [Brownian motion](../../../../../../brownian-motion-split.md). If $d_\alpha$ is the lower $\alpha$-quantile of $D$, the **asymptotic level-$\alpha$ critical region** is

$$
\boxed{T_n<d_\alpha.}
$$

The deterministic terms and null initialization must match the critical-value table. For exact finite-sample [size of a statistical test](../../../../../../size-of-a-statistical-test.md), calibrate the statistic from its Gaussian [random walk](../../../../../../random-walk.md) null with the specified initial condition and noise scale; for a zero starting value its distribution is scale-free. The printed two-sided recurrence alone specifies neither an initial law nor a universal finite-sample critical value. Ordinary normal quantiles do not give the intended [size of a statistical test](../../../../../../size-of-a-statistical-test.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
