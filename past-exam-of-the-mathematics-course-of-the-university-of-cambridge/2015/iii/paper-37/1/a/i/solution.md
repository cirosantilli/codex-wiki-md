<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**A stationary [causal time series](../../../../../../../causal-time-series.md) exists.** The [infinite moving-average representation](../../../../../../../infinite-moving-average-representation.md)

$$
X_t=\sum_{j=0}^\infty 2^{-j}\varepsilon_{t-j}
$$

converges in the sense of [mean-square convergence](../../../../../../../convergence-in-l2.md) because the driving variables are [independent random variables](../../../../../../../independent-random-variables.md) and $\sum_j4^{-j}<\infty$. Shifting the series gives $X_t=\tfrac12X_{t-1}+\varepsilon_t$. Its [expected value](../../../../../../../expected-value.md) is zero and its [autocovariance](../../../../../../../autocovariance.md) is

$$
\boxed{\gamma(h)=\frac{4\sigma^2}{3}\,2^{-|h|}.}
$$

Thus it is a [weakly stationary process](../../../../../../../weakly-stationary-process.md); since the driving variables have a [normal distribution](../../../../../../../normal-distribution.md), it is also a [Gaussian process](../../../../../../../gaussian-process.md) and a [strictly stationary process](../../../../../../../strictly-stationary-process.md). Throughout the stationarity discussion, take $\sigma^2>0$; degenerate zero noise permits trivial constant solutions.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
