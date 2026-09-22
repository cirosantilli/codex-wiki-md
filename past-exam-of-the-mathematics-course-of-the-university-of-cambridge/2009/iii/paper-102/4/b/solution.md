<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a population-averaged rate trend, use the [marginal incidence trend with clustered observations](../../../../../../marginal-incidence-trend-with-clustered-observations.md) model

$$
\boxed{\log\mathbb E[Y_{it}]=\log P_{it}+\alpha+\beta t,\qquad t=0,\ldots,4.}
$$

Fit a [generalized estimating equation](../../../../../../generalized-estimating-equation.md) with village as cluster, a log link and an appropriate working correlation; estimate uncertainty with a village-level [sandwich covariance matrix](../../../../../../sandwich-covariance-matrix.md). Then $e^\beta$ is the fitted annual marginal [rate ratio](../../../../../../rate-ratio.md), $100(e^\beta-1)$ is the annual percentage rate change, and $e^{4\beta}$ is the four-year endpoint ratio. Test $\beta=0$ using cluster-robust uncertainty, with a small-sample correction or village-resampling [bootstrap](../../../../../../bootstrapping-statistics.md) given only 32 independent clusters. Also compare year as a factor with a linear trend, since a single slope can conceal nonlinear behaviour.

Report which population is averaged over. The directly pooled rate $\sum_iY_{it}/\sum_iP_{it}$ is exposure weighted; a mean of village rates gives each village equal weight. For standardized comparisons one can use the same village weights at every year, preventing changing population composition from masquerading as a rate trend.

A conditional random-slope coefficient cannot simply be substituted for the marginal slope: the [marginal mean of a Poisson random-slope model](../../../../../../marginal-mean-of-a-poisson-random-slope-model.md) contains time-dependent variance terms. **A direction, magnitude and confidence interval for the trend across all villages require the missing full dataset.** The increase in the two displayed villages does not determine the trend in the other thirty.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
