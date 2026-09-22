<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume positive deterministic initial stock prices and finite, positive terminal [variances](../../../../../../variance-split.md), as required to define the [correlation coefficient](../../../../../../pearson-correlation-coefficient.md). The explicit stochastic-exponential solutions with constant volatilities give

$$
\frac{S_t}{S'_t}=\frac{S_0}{S'_0}\exp\left[(\sigma-\sigma')B_t-\tfrac12(\sigma^2-(\sigma')^2)t\right].
$$

The common, possibly random, accumulated interest rate cancels. If $\sigma=\sigma'$, this ratio is a positive constant, so the prices are perfectly correlated.

Conversely, perfect correlation would give $S_t=cS'_t+d$ almost surely for constants $c>0,d$. If $\sigma\ne\sigma'$, the displayed ratio is a nonconstant variable with a [lognormal distribution](../../../../../../log-normal-distribution.md) with full support $(0,\infty)$. If $d>0$, the ratio would always exceed $c$, and if $d<0$ it would always be below $c$, both impossible. If $d=0$, the ratio would be constant, also impossible. **Therefore $\boxed{\rho(S_t,S'_t)=1\iff\sigma=\sigma'}$**, whenever the stated terminal [variances](../../../../../../variance-split.md) exist and are positive. No deterministic-interest assumption is needed. Degenerate terminal prices, for example zero volatilities and deterministic rates, have undefined correlation and must be excluded.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
