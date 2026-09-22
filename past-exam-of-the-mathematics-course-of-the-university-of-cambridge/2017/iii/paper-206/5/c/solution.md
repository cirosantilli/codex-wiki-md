<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A zero-mean [autoregressive process of order one](../../../../../../autoregressive-process-of-order-one.md) satisfies

$$
Y_t=\alpha Y_{t-1}+\varepsilon_t,
$$

where $\varepsilon_t$ is [white noise](../../../../../../white-noise.md) with [variance](../../../../../../variance-split.md) $\sigma_\varepsilon^2>0$. A [causal time series](../../../../../../causal-time-series.md) uses present and past innovations only. For $|\alpha|<1$ the series

$$
Y_t=\sum_{j=0}^\infty\alpha^j\varepsilon_{t-j}
$$

has [mean-square convergence](../../../../../../convergence-in-l2.md) because $\sum_j\alpha^{2j}<\infty$, and it supplies the causal [weakly stationary process](../../../../../../weakly-stationary-process.md). Its [variance](../../../../../../variance-split.md) is $\sigma_\varepsilon^2/(1-\alpha^2)$. For $h\ge0$, only the common innovations contribute to the [autocovariance](../../../../../../autocovariance.md):

$$
\gamma(h)=\sigma_\varepsilon^2\sum_{j=0}^\infty\alpha^{h+j}\alpha^j=\frac{\sigma_\varepsilon^2\alpha^h}{1-\alpha^2}.
$$

Evenness then gives

$$
\boxed{\gamma(h)=\frac{\sigma_\varepsilon^2\alpha^{|h|}}{1-\alpha^2},\qquad \rho(h)=\alpha^{|h|}.}
$$

When $\alpha<0$, the signs alternate; when $\alpha=0$, the process is white noise. With nondegenerate innovations, $|\alpha|\ge1$ does not give a causal finite-variance stationary solution. These [covariance](../../../../../../covariance.md) calculations need uncorrelated innovations, not Gaussianity; Gaussian innovations additionally yield a Gaussian process.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
