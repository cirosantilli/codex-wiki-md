<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**A [noncausal stationary autoregression](../../../../../../../noncausal-stationary-autoregression.md) exists.** On the two-sided time axis define

$$
X_t=-\sum_{j=1}^\infty2^{-j}\varepsilon_{t+j}.
$$

This series converges in the sense of [mean-square convergence](../../../../../../../convergence-in-l2.md), and direct subtraction gives $X_t-2X_{t-1}=\varepsilon_t$. The [expected value](../../../../../../../expected-value.md) and [autocovariance](../../../../../../../autocovariance.md) are

$$
\boxed{\mathbb EX_t=0,\qquad\gamma(h)=\frac{\sigma^2}{3}\,2^{-|h|}.}
$$

Consequently this is a [weakly stationary process](../../../../../../../weakly-stationary-process.md) and, by Gaussianity, a [strictly stationary process](../../../../../../../strictly-stationary-process.md). It is an example of [noncausal stationary autoregression](../../../../../../../noncausal-stationary-autoregression.md), since $X_t$ uses future noise. In particular, $X_{t-1}$ is correlated with $\varepsilon_t$, so the usual causal [variance](../../../../../../../variance-split.md) recursion is inapplicable. If an additional assumption required the driving noise to be independent of past observations, this solution would be excluded; that assumption is not stated here.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
