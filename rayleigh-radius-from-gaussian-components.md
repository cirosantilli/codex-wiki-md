# Rayleigh radius from Gaussian components

↑ **Parent:** [Rayleigh distribution](rayleigh-distribution.md)

The [joint probability density](joint-probability-density.md) of $X,Y$ is

$$
p(x,y)=\frac1{2\pi\sigma^2}e^{-(x^2+y^2)/(2\sigma^2)}.
$$

In [polar coordinates](polar-coordinates.md), $x=r\cos\theta$, $y=r\sin\theta$, and the absolute [Jacobian determinant](jacobian-determinant.md) is $r$. Thus the joint density of [radius](radius.md) and angle factors as

$$
p_{R,\Theta}(r,\theta)=\frac r{\sigma^2}e^{-r^2/(2\sigma^2)}\frac1{2\pi},\qquad r>0,\quad0\leq\theta<2\pi.
$$

Integrating over angle gives the [Rayleigh distribution](rayleigh-distribution.md). The same factorization shows that the angle has [uniform distribution](continuous-uniform-distribution.md) and is [independent](independent-random-variables.md) of the [radius](radius.md). This is a short [change of variables](change-of-variables-formula.md) argument: an [annulus](annulus-mathematics.md) of width $dr$ has [area](surface-area.md) $2\pi r\,dr$ to first order.

The assumptions are substantive. Unequal component [variances](variance-split.md) give elliptical rather than circular density contours; a nonzero mean displaces the center. Even zero [covariance](covariance.md) and equal [normal distributions](normal-distribution.md) do not suffice without [independence](independent-random-variables.md). For an original counterexample, let $X\sim N(0,\sigma^2)$ and let $S$ be an [independent](independent-random-variables.md) [Rademacher random variable](rademacher-distribution.md). Put $Y=SX$. Then $Y$ has the same [normal distribution](normal-distribution.md) as $X$, and $\operatorname{Cov}(X,Y)=\mathbb E[SX^2]=0$. Nevertheless, all points lie on $y=x$ or $y=-x$, and $R=\sqrt2|X|$ has density

$$
f_R(r)=\frac1{\sigma\sqrt\pi}e^{-r^2/(4\sigma^2)},\qquad r\geq0,
$$

which is positive at zero, unlike the [Rayleigh distribution](rayleigh-distribution.md). This pair is not a [Gaussian random vector](gaussian-random-vector.md).

## ↑ Ancestors (8)

1. [Rayleigh distribution](rayleigh-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
