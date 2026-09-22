# Boundary bias of a kernel density estimator

↑ **Parent:** [Bias of a kernel density estimator](bias-of-a-kernel-density-estimator.md)

If the unknown [probability distribution](probability-distribution-split.md) is supported on $[0,\infty)$, an ordinary [Gaussian density kernel](gaussian-density-kernel.md) still puts some fitted [probability](probability.md) below zero. For positive observations $X_i$ and the [standard normal distribution](standard-normal-distribution.md) [cumulative distribution function](cumulative-distribution-function.md) $\Phi$, the displayed formula gives the total leakage. For the [statistical sample](statistical-sample.md) $(0.1,0.4,0.9)$ and [smoothing bandwidth](smoothing-bandwidth.md) $h=0.5$, it is

$$
\frac{\Phi(-0.2)+\Phi(-0.8)+\Phi(-1.8)}3=\frac{0.42074029+0.21185540+0.03593032}{3}=0.22284200\ldots.
$$

Thus about $22.28\%$ of the fitted [probability](probability.md) falls outside the known [support of a probability distribution](support-of-a-probability-distribution.md), even though the full [integral](integral-split.md) remains one. The leakage panel in [smoothing bandwidth](smoothing-bandwidth.md) shades this area. Simply deleting the negative part leaves area $0.777158\ldots$; renormalizing it makes another [probability density function](probability-density-function.md) but does not by itself establish that the [bias of an estimator](bias-of-an-estimator.md) has been corrected.

The issue also appears in the [expectation](expected-value-split.md) of the [kernel density estimator](kernel-density-estimation.md). For a nonnegative symmetric [kernel for density estimation](kernel-for-density-estimation.md) and a [probability density function](probability-density-function.md) $f$ that is zero for $x<0$ and has a finite positive right-hand limit $f(0+)$, assume $f$ is bounded. Then, for fixed $K$ as $h\downarrow0$,

$$
\mathbb E\widehat f_h(0)=\int_0^\infty K(u)f(hu)\,du\longrightarrow\frac12 f(0+).
$$

Half the averaging window lies on the impossible side of the boundary. For example, the rate-one [exponential distribution](exponential-distribution.md) has $f(0+)=1$, so the limiting expected boundary height is $1/2$, rather than the right-hand height one. This refers to estimating the right-hand limit; changing a [probability density function](probability-density-function.md) at a single point does not change its [probability distribution](probability-distribution-split.md). Decreasing the [smoothing bandwidth](smoothing-bandwidth.md) narrows the affected region but does not remove this boundary-height error. This is why the interior [second-order pointwise bias bound for kernel density estimation](second-order-pointwise-bias-bound-for-kernel-density-estimation.md) cannot be applied across a jump at the boundary.

## ↑ Ancestors (10)

1. [Bias of a kernel density estimator](bias-of-a-kernel-density-estimator.md)
2. [Kernel density estimation](kernel-density-estimation.md)
3. [Kernel for density estimation](kernel-for-density-estimation.md)
4. [Density estimation](density-estimation.md)
5. [Nonparametric statistics](nonparametric-statistics-split.md)
6. [Statistical inference](statistical-inference-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Smoothing bandwidth](smoothing-bandwidth.md)
