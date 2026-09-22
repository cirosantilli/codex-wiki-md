# Rayleigh moments

↑ **Parent:** [Rayleigh distribution](rayleigh-distribution.md)

Using $u=r^2/(2\sigma^2)$ in the defining [expected value](expected-value-split.md) integral gives

$$
\mathbb E[R^q]
=\int_0^\infty r^q\frac r{\sigma^2}e^{-r^2/(2\sigma^2)}\,dr
=\sigma^q2^{q/2}\int_0^\infty u^{q/2}e^{-u}\,du
=\sigma^q2^{q/2}\Gamma(1+q/2),\qquad q>-2.
$$

The last integral is the [gamma function](gamma-function.md). Near zero, the integrand before substitution behaves as $r^{q+1}$, explaining the threshold $q>-2$; at infinity the Gaussian tail controls every power. In particular,

$$
\mathbb E[R]=\sigma\sqrt{\frac\pi2},\quad
\mathbb E[R^2]=2\sigma^2,\quad
\operatorname{Var}(R)=\left(2-\frac\pi2\right)\sigma^2.
$$

[Random: Probability, Mathematical Statistics, Stochastic Processes by Kyle Siegrist; The General Rayleigh Distribution, Moments: mean, variance and nonnegative integer moments; extension to real q greater than -2 follows from the displayed integral](random-probability-mathematical-statistics-stochastic-processes-by-kyle-siegrist/the-rayleigh-distribution.md)

For the chosen $\sigma=2\,\mathrm{cm}$, the [mean](expected-value-split.md) [radius](radius.md) is about $2.5066\,\mathrm{cm}$, its [median](median.md) is $2\sqrt{2\log2}\simeq2.3548\,\mathrm{cm}$, and its [mode](mode-statistics.md) is $2\,\mathrm{cm}$. Its [root mean square](root-mean-square.md) is $2\sqrt2\simeq2.8284\,\mathrm{cm}$. Different summaries answer different questions; the component scale $\sigma$ is neither the radial [mean](expected-value-split.md) nor the radial [standard deviation](standard-deviation.md).

## ↑ Ancestors (8)

1. [Rayleigh distribution](rayleigh-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
