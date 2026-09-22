# Polar decomposition of a planar standard normal vector

↑ **Parent:** [Multivariate Gaussian distribution](multivariate-gaussian-distribution.md)

For [independent](independent-random-variables.md) [standard normal random variables](standard-normal-random-variable.md) $X,Y$, put $X=R\cos\Theta$, $Y=R\sin\Theta$, with $R\geq0$ and $0\leq\Theta<2\pi$. The [polar coordinates](polar-coordinates.md) [Jacobian determinant](jacobian-determinant.md) is $r$, so the [joint probability density](joint-probability-density.md) is $r e^{-r^2/2}/(2\pi)$ on $r>0$. It factorizes into a [Rayleigh distribution](rayleigh-distribution.md) density for $R$ and a [continuous uniform distribution](continuous-uniform-distribution.md) density for $\Theta$. Consequently the radius and angle are [independent](independent-random-variables.md). The [change of variables for probability densities](change-of-variables-for-probability-densities.md) $S=R^2$ gives $f_S(s)=e^{-s/2}/2$ for $s>0$, the [exponential distribution](exponential-distribution.md) of rate $1/2$, also the [chi-squared distribution](chi-squared-distribution.md) with two degrees of freedom. Measurable transformation preserves [independence](independent-random-variables.md), giving $\Theta\perp S$. The angle at $R=0$ is arbitrary on an event of [probability](probability.md) zero.

Thus a sector with angular length $\ell$ has [probability](probability.md) $\ell/(2\pi)$, independently of any radial restriction. For instance $Y>|X|$ occupies a sector of angle $\pi/2$ and has [probability](probability.md) $1/4$.

## ↑ Ancestors (8)

1. [Multivariate Gaussian distribution](multivariate-gaussian-distribution.md)
2. [Normal distribution](normal-distribution.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2015/2/a/i/solution.md)
