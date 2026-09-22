# Squared Rayleigh radius

↑ **Parent:** [Rayleigh distribution](rayleigh-distribution.md)

Squaring a [Rayleigh distribution](rayleigh-distribution.md) variable produces an [exponential distribution](exponential-distribution.md). For $w\geq0$,

$$
\mathbb P(R^2>w)=e^{-w/(2\sigma^2)},\qquad
R^2\sim\operatorname{Exp}\left(\frac1{2\sigma^2}\right),
$$

where the [exponential distribution](exponential-distribution.md) parameter is a rate. Equivalently, $R^2/\sigma^2$ has [chi-squared distribution](chi-squared-distribution.md) with two [degrees of freedom (statistics)](statistical-degrees-of-freedom.md). An amplitude and its square therefore have different [probability density functions](probability-density-function.md), even though one determines the other.

This makes the [Rayleigh-normal scale mixture](rayleigh-normal-scale-mixture.md) transparent: at unit scale, $R^2$ is exponential, allowing a random normal scale to produce a [Laplace distribution](laplace-distribution.md). Another equivalent parametrization uses a [Weibull distribution](weibull-distribution.md) with shape two and scale $\sqrt2\sigma$. Conventions that call this latter scale the Rayleigh scale differ by a factor of $\sqrt2$; check the [probability density function](probability-density-function.md) before comparing numerical parameter values.[NIST Dataplot Reference Manual; Description: chi distribution with two degrees of freedom; Weibull shape two and scale sqrt(2) times sigma; warning about Rayleigh scale conventions](nist-dataplot-reference-manual/rayleigh-probability-density-function.md)

## ↑ Ancestors (8)

1. [Rayleigh distribution](rayleigh-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
