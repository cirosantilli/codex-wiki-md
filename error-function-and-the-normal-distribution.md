# Error function and the normal distribution

↑ **Parent:** [Error function](error-function.md)

For a [standard normal random variable](standard-normal-random-variable.md) $Z$, its [standard normal distribution function](standard-normal-distribution-function.md) is

$$
\Phi(z)=\frac{1}{\sqrt{2\pi}}\int_{-\infty}^{z}e^{-u^2/2}\,du
=\frac12\left[1+\operatorname{erf}\!\left(\frac{z}{\sqrt2}\right)\right].
$$

The [change of variables](change-of-variables-formula.md) $t=u/\sqrt2$ and the [symmetric distribution](symmetric-distribution.md) of the [standard normal random variable](standard-normal-random-variable.md) give the second expression. For $X\sim N(\mu,\sigma^2)$ with $\sigma>0$, [standardization of a normal random variable](standardization-of-a-normal-random-variable.md) then gives

$$
\mathbb P(X\le x)=\frac12\left[1+\operatorname{erf}\!\left(\frac{x-\mu}{\sigma\sqrt2}\right)\right],\qquad
\mathbb P(|X-\mu|\le a\sigma)=\operatorname{erf}\!\left(\frac{a}{\sqrt2}\right),\quad a\ge0.
$$

In particular, the intervals within one, two, and three [standard deviations](standard-deviation.md) have calculated [probabilities](probability.md) about $0.682689$, $0.954500$, and $0.997300$. These values depend on a [normal distribution](normal-distribution.md); they are not universal coverage guarantees for an arbitrary [random variable](random-variable-split.md). This is the direct connection between a [Gaussian function](gaussian-function.md) area and the familiar central intervals.

For a small upper-tail [probability](probability.md), use the [complementary error function](complementary-error-function.md) directly:

$$
\boxed{\mathbb P(Z>z)=\frac12\operatorname{erfc}\!\left(\frac{z}{\sqrt2}\right).}
$$

Computing this as $1-\Phi(z)$ instead can lose the tail to [catastrophic cancellation](catastrophic-cancellation.md). The [Gaussian tail bound](gaussian-tail-bound.md) gives another useful estimate without requiring an exact [error function](error-function.md) value.

## ↑ Ancestors (9)

1. [Error function](error-function.md)
2. [Gaussian integral](gaussian-integral.md)
3. [Integral](integral-split.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Error function](error-function.md)
