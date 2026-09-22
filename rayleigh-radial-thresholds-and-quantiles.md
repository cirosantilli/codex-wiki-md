# Rayleigh radial thresholds and quantiles

↑ **Parent:** [Rayleigh distribution](rayleigh-distribution.md)

For $r\geq0$, integration gives the [survival function](survival-function.md) and [cumulative distribution function](cumulative-distribution-function.md)

$$
\mathbb P(R>r)=e^{-r^2/(2\sigma^2)},\qquad
F_R(r)=1-e^{-r^2/(2\sigma^2)}.
$$

Solving $F_R(r_p)=p$ gives the [quantile function](quantile-function.md)

$$
\boxed{r_p=\sigma\sqrt{-2\log(1-p)},\qquad0<p<1.}
$$

[Random: Probability, Mathematical Statistics, Stochastic Processes by Kyle Siegrist; The General Rayleigh Distribution, Distribution Functions: CDF, quantile and survival functions](random-probability-mathematical-statistics-stochastic-processes-by-kyle-siegrist/the-rayleigh-distribution.md)

For the chosen positioning model $\sigma=2\,\mathrm{cm}$,

$$
\mathbb P(R\leq2\,\mathrm{cm})=1-e^{-1/2}\simeq0.3935,\qquad
\mathbb P(R\leq4\,\mathrm{cm})=1-e^{-2}\simeq0.8647.
$$

The [disk](disk-mathematics.md) of [radius](radius.md) one component [standard deviation](standard-deviation.md) therefore contains about 39.35% of outcomes; the familiar one-dimensional normal interval percentage does not apply to a two-dimensional [disk](disk-mathematics.md). The 95% and 99% radial thresholds are

$$
\boxed{r_{0.95}\simeq4.8955\,\mathrm{cm},\qquad r_{0.99}\simeq6.0697\,\mathrm{cm}.}
$$

A [circle](circle.md) defined by $R=r_p$ itself still has [probability](probability.md) zero; its enclosed [disk](disk-mathematics.md) carries the stated [probability](probability.md).

<a id="image-radial-coverage-uses-disks-rather-than-one-dimensional-normal-intervals"></a>
![](rayleigh-radius-coverage-and-thresholds.png)

**[Figure 6](#image-radial-coverage-uses-disks-rather-than-one-dimensional-normal-intervals). Radial coverage uses disks rather than one-dimensional normal intervals**. Original chosen model: each independent centered coordinate has [standard deviation](standard-deviation.md) $2\,\mathrm{cm}$. Concentric [disks](disk-mathematics.md) have radii $2\,\mathrm{cm}$, $4\,\mathrm{cm}$ and the calculated 95% threshold $4.8955\,\mathrm{cm}$. The curve gives exact model coverage, not empirical counts.

The closed-form [quantile function](quantile-function.md) also gives [inverse transform sampling](inverse-transform-sampling.md): if $U$ has [uniform distribution](continuous-uniform-distribution.md) on $(0,1)$, then $\sigma\sqrt{-2\log U}$ has [Rayleigh distribution](rayleigh-distribution.md). Using $1-U$ instead gives the same law. Endpoints are excluded so that the [logarithm](logarithm.md) stays finite.

## ↑ Ancestors (8)

1. [Rayleigh distribution](rayleigh-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
