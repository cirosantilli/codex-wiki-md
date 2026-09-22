# Rayleigh distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rayleigh_distribution)

The [Rayleigh distribution](rayleigh-distribution.md) is the [probability distribution](probability-distribution-split.md) of the [Euclidean norm](euclidean-norm.md) of a two-dimensional [random vector](random-vector.md) with [independent](independent-random-variables.md) zero-[mean](expected-value-split.md) [normal random variables](gaussian-random-variable.md) of equal [variance](variance-split.md) as components. If $X,Y\sim N(0,\sigma^2)$ are [independent](independent-random-variables.md), then

$$
R=\sqrt{X^2+Y^2}\sim\operatorname{Rayleigh}(\sigma),\qquad
f_R(r)=\begin{cases}\dfrac r{\sigma^2}e^{-r^2/(2\sigma^2)},&r\geq0,\\0,&r<0.\end{cases}
$$

Here $\sigma$ is the [standard deviation](standard-deviation.md) of each component, not of the [radius](radius.md) $R$. At $\sigma=1$ this gives the unit-scale [probability density function](probability-density-function.md) $r e^{-r^2/2}$.[Random: Probability, Mathematical Statistics, Stochastic Processes by Kyle Siegrist; The General Rayleigh Distribution, Definition and Distribution Functions: independent equal-scale centered normal components and radial density](random-probability-mathematical-statistics-stochastic-processes-by-kyle-siegrist/the-rayleigh-distribution.md)

This geometry turns two signed errors into one nonnegative distance. For example, suppose horizontal and vertical positioning errors are [independent](independent-random-variables.md) $N(0,4\,\mathrm{cm}^2)$ [random variables](random-variable-split.md). Their [means](expected-value-split.md) both vanish, but the distance from the intended point is usually positive. The [Rayleigh distribution](rayleigh-distribution.md) with $\sigma=2\,\mathrm{cm}$ gives the [probability](probability.md) of landing inside any centered [disk](disk-mathematics.md). These are chosen model assumptions, rather than measurements of a particular instrument.

<a id="image-the-center-maximizes-planar-density-while-a-positive-radius-maximizes-radial-density"></a>
![](rayleigh-gaussian-area-and-radius.png)

**[Figure 5](#image-the-center-maximizes-planar-density-while-a-positive-radius-maximizes-radial-density). The center maximizes planar density, while a positive radius maximizes radial density**. Original calculated model with $\sigma=1$. Left: [joint probability density](joint-probability-density.md) per unit [area](surface-area.md), with an [annulus](annulus-mathematics.md) from $r=0.9$ to $r=1.1$. Right: [probability density function](probability-density-function.md) per unit [radius](radius.md); the shaded area is the probability of that same [annulus](annulus-mathematics.md). A single point and a single [circle](circle.md) both have probability zero.

An apparently paradoxical feature is that the most likely location per unit [area](surface-area.md) is the origin, while the radial [mode](mode-statistics.md) is $\sigma$. A narrow [annulus](annulus-mathematics.md) farther out has more [area](surface-area.md). Near zero that growing [circumference](circumference.md) outweighs the falling planar density; farther out the [exponential function](exponential-function.md) wins. Distinguishing densities measured against different elements of [area](surface-area.md) or length resolves the paradox.

**Table of contents**

- [Rayleigh radius from Gaussian components](rayleigh-radius-from-gaussian-components.md)
- [Rayleigh radial thresholds and quantiles](rayleigh-radial-thresholds-and-quantiles.md)
- [Squared Rayleigh radius](squared-rayleigh-radius.md)
- [Rayleigh moments](rayleigh-moments.md)
- [Random-phase amplitude and the Rayleigh distribution](random-phase-amplitude-and-the-rayleigh-distribution.md)

## ↑ Ancestors (7)

1. [Continuous probability distribution](continuous-probability-distribution-split.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Circumference](circumference.md)
- [Gaussian-over-Rayleigh inclination distribution](gaussian-over-rayleigh-inclination-distribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-51/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/4/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/4/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/11/b/solution.md)
- [Random-phase amplitude and the Rayleigh distribution](random-phase-amplitude-and-the-rayleigh-distribution.md)
- [Rayleigh distribution](rayleigh-distribution.md)
- [Rayleigh-normal scale mixture](rayleigh-normal-scale-mixture.md)
- [Rayleigh radial thresholds and quantiles](rayleigh-radial-thresholds-and-quantiles.md)
- [Rayleigh radius from Gaussian components](rayleigh-radius-from-gaussian-components.md)
- [Squared Rayleigh radius](squared-rayleigh-radius.md)
