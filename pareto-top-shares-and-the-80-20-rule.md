<h1 id="pareto-top-shares-and-the-80-20-rule">Pareto top shares and the 80/20 rule</h1>

↑ **Parent:** [Pareto distribution](pareto-distribution.md)

For a nonnegative [random variable](random-variable-split.md) with finite positive [mean](expected-value-split.md), the share of its total amount carried by the largest fraction $q$ of outcomes can be defined by dividing their contribution to the [expected value](expected-value-split.md) by the whole [expected value](expected-value-split.md). For a [Pareto distribution](pareto-distribution.md), let $0<q\leq1$ and choose $x_q=\beta q^{-1/\alpha}$, so that $\mathbb P(X\geq x_q)=q$. If $\alpha>1$, direct integration gives

$$
T(q)=\frac{\mathbb E[X\mathbf1_{\{X\geq x_q\}}]}{\mathbb E[X]}
=\frac{\alpha\beta^\alpha x_q^{1-\alpha}/(\alpha-1)}{\alpha\beta/(\alpha-1)}
=q^{1-1/\alpha}.
$$

This is a share of amount, distinct from the fraction of outcomes. It depends on $\alpha$, but not on the unit of measurement $\beta$.[Section III.D, pp. 10–11, Eqs. (27)–(28): upper-population share; Newman's density exponent equals alpha+1 in the present tail-exponent convention](power-laws-pareto-distributions-and-zipf-s-law-by-mark-newman.md)

For the chosen $\alpha=2$, the top 20% starts at $x_{0.2}=10\sqrt5\simeq22.361$ and carries $T(0.2)=\sqrt{0.2}\simeq44.72\%$ of the amount. To make the top 20% carry exactly 80%, solve

$$
(1/5)^{1-1/\alpha}=4/5
\quad\Longrightarrow\quad
\alpha=\frac{\log5}{\log4}\simeq1.160964.
$$

The resulting [Pareto distribution](pareto-distribution.md) has a finite [mean](expected-value-split.md) and infinite [variance](variance-split.md). The 80/20 rule selects one [shape parameter](shape-parameter.md); it is not a universal law, or even a property of every [Pareto distribution](pareto-distribution.md). For $\alpha\leq1$, the population-share definition above is unavailable because its denominator is infinite; substituting such an $\alpha$ into the finite-mean formula is invalid.

<a id="image-changing-pareto-alpha-changes-quantiles-moment-existence-and-the-top-20-percent-share"></a>
![](pareto-alpha-quantiles-and-top-share.png)

**[Figure 4](#image-changing-pareto-alpha-changes-quantiles-moment-existence-and-the-top-20-percent-share). Changing Pareto alpha changes quantiles, moment existence and the top 20 percent share**.

The left panel compares three [quantiles](quantile-function.md) in units of the minimum. The right panel shows $T(0.2)$ only where the [mean](expected-value-split.md) is finite, and marks the chosen 80/20 value. The thresholds $\alpha=1$ and $\alpha=2$ separate the [moment](moment.md) regimes; they do not separate valid and invalid [probability distributions](probability-distribution-split.md).

A straight-looking empirical [log-log plot](log-log-plot.md) does not by itself establish a [Pareto distribution](pareto-distribution.md) or a reliable tail exponent; estimating an exponent and assessing [goodness of fit](goodness-of-fit.md) are separate tasks.[Section II, pp. 4–5, Eqs. (3)–(5) and discussion: survival versus density exponent, biases from fitting plotted slopes, and the lower threshold for power-law behaviour](power-laws-pareto-distributions-and-zipf-s-law-by-mark-newman.md) If a [Pareto distribution](pareto-distribution.md) is used only above a fitted lower threshold, $T(q)$ describes that conditional tail population, not automatically the whole population. A genuine finite upper cutoff gives a [truncated distribution](truncated-distribution.md) with finite nonnegative [moments](moment.md); its [survival function](survival-function.md), [quantiles](quantile-function.md) and top shares must be recalculated. Truncation is a modelling change, distinct from merely observing a finite sample. None of the chosen numbers here estimates an actual wealth distribution.

## ↑ Ancestors (8)

1. [Pareto distribution](pareto-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
