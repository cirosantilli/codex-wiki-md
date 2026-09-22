<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the following form of the [Girsanov theorem](../../../../../../girsanov-theorem.md). If $W$ is [Brownian motion](../../../../../../brownian-motion-split.md), $\vartheta$ is predictable, and

$$
Z_t=\exp\left(\int_0^t\vartheta_s\,dW_s-\frac12\int_0^t\vartheta_s^2\,ds\right)
$$

is a [uniformly integrable martingale](../../../../../../uniformly-integrable-martingale.md) with $Z_0=1$, then the [probability measure](../../../../../../probability-measure.md) with terminal density $Z_\infty$ makes $W_t-\int_0^t\vartheta_s\,ds$ a [Brownian motion](../../../../../../brownian-motion-split.md). The analogous finite-horizon statement uses the terminal density at that horizon.

Here take $W_t=X_t-x$ and $\vartheta_s=\mathbf1_{\{s<\tau\}}/X_s$. Before $\tau$, $X_s\in[\varepsilon,M]$, so the [stochastic integral](../../../../../../stochastic-integral.md) is well-defined. The assumed uniform integrability of the stopped [stochastic exponential](../../../../../../doleans-dade-exponential.md) gives

$$
\mathbb E_{\mathbb W_x}Z_\tau=1,\qquad
Z_{t\wedge\tau}=\mathbb E_{\mathbb W_x}(Z_\tau\mid\mathcal F_t).
$$

Thus the proposed weighting really defines a [probability measure](../../../../../../probability-measure.md), and the [Girsanov theorem](../../../../../../girsanov-theorem.md) gives the [Brownian motion](../../../../../../brownian-motion-split.md)

$$
B_t=X_t-x-\int_0^{t\wedge\tau}\frac{ds}{X_s}
$$

under that measure. In particular

$$
\boxed{X_t=x+B_t+\int_0^t\frac{ds}{X_s}\qquad(0\le t\le\tau).}
$$

All calculations are first made on this compact stopped interval. The integral involving $1/X$ is naturally defined on $[0,T_0)$; at $T_0$ its [quadratic variation](../../../../../../quadratic-variation.md) may diverge. The density will have a zero limiting extension there, as established below, rather than a finite stochastic logarithm at the hitting time.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
