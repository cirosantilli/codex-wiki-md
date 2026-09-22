# Pareto tail conditional scaling

↑ **Parent:** [Pareto distribution](pareto-distribution.md)

Conditioning a [Pareto distribution](pareto-distribution.md) on exceeding a threshold changes its minimum while preserving its [shape parameter](shape-parameter.md). For $u\geq\beta$ and $x\geq u$, the definition of [conditional probability](conditional-probability.md) gives

$$
\mathbb P(X>x\mid X\geq u)=\frac{(\beta/x)^\alpha}{(\beta/u)^\alpha}=\left(\frac{u}{x}\right)^\alpha.
$$

Equivalently, for $r\geq1$,

$$
\mathbb P(X/u>r\mid X\geq u)=r^{-\alpha}.
$$

The ratio to the threshold has the same [Pareto distribution](pareto-distribution.md) at every admissible threshold.[Random: Probability, Mathematical Statistics, Stochastic Processes by Kyle Siegrist; The General Pareto Distribution, Related Distributions: closure under right-tail conditioning](random-probability-mathematical-statistics-stochastic-processes-by-kyle-siegrist/the-pareto-distribution.md) For the chosen $\alpha=2$, $\beta=10$, only $1/4$ of outcomes exceed 20, but among those outcomes the [probability](probability.md) of exceeding 40 is again $1/4$. When $\alpha>1$, the same identity gives [conditional expectation](conditional-expectation.md) $\mathbb E[X\mid X\geq u]=\alpha u/(\alpha-1)$.

This multiplicative scaling differs from the additive [memoryless property](memorylessness-of-the-exponential-distribution.md) of an [exponential distribution](exponential-distribution.md). Indeed $Y=\log(X/\beta)$ has [exponential distribution](exponential-distribution.md) of rate $\alpha$, because $\mathbb P(Y>y)=e^{-\alpha y}$ for $y\geq0$. Thus logarithms turn multiplication into addition and explain the scaling property. Conversely, if $U$ has [uniform distribution](continuous-uniform-distribution.md) on $(0,1)$, [inverse transform sampling](inverse-transform-sampling.md) gives $X=\beta(1-U)^{-1/\alpha}$.

The excess $Z=X-u$ conditional on $X\geq u$ has [survival function](survival-function.md) $(1+z/u)^{-\alpha}$ for $z\geq0$. In the [generalized Pareto distribution](generalized-pareto-distribution.md) convention $\mathbb P(Z>z)=(1+\xi z/\sigma)^{-1/\xi}$, this means $\xi=1/\alpha$ and $\sigma=u/\alpha$. Here the excess starts at zero; the original [Pareto distribution](pareto-distribution.md) starts at $\beta>0$.

## ↑ Ancestors (8)

1. [Pareto distribution](pareto-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
