# Arcsine quantiles and moments

↑ **Parent:** [Arcsine distribution](arcsine-distribution.md)

Inverting $F(x)=p$ gives the [quantile function](quantile-function.md)

$$
Q(p)=\sin^2\left(\frac{\pi p}{2}\right),\qquad0\leq p\leq1.
$$

Consequently, [inverse transform sampling](inverse-transform-sampling.md) uses $X=\sin^2(\pi U/2)$ with $U$ uniform on $(0,1)$. The [quartiles](quartile.md) are $(2-\sqrt2)/4$, $1/2$ and $(2+\sqrt2)/4$.[Random: Probability, Mathematical Statistics, Stochastic Processes by Kyle Siegrist; The Standard Arcsine Distribution, Distribution Functions and Related Distributions: quantiles, quartiles and random quantile construction](random-probability-mathematical-statistics-stochastic-processes-by-kyle-siegrist/the-arcsine-distribution.md)

The first and third [quartiles](quartile.md) are about $0.1464$ and $0.8536$, so the central half of the [probability](probability.md) spans about $0.7071$ of the unit interval. Under a [uniform distribution](continuous-uniform-distribution.md), its width would be $0.5$.

The [symmetric probability distribution](symmetric-probability-distribution.md) gives $\mathbb E[X]=1/2$. The angle representation gives a short calculation of the second [moment](moment.md):

$$
\mathbb E[X^2]=\frac2\pi\int_0^{\pi/2}\sin^4\theta\,d\theta=\frac38,
\qquad \operatorname{Var}(X)=\frac38-\frac14=\frac18.
$$

Use $\sin^4\theta=(3-4\cos2\theta+\cos4\theta)/8$ to evaluate the integral. A [uniform distribution](continuous-uniform-distribution.md) on $[0,1]$ has [variance](variance-split.md) $1/12$; the larger [variance](variance-split.md) $1/8$ quantifies the greater spread toward the ends.

More generally, for a nonnegative [integer](integer-split.md) $n$, the [beta function](beta-function.md) yields

$$
\mathbb E[X^n]=\frac{B(n+1/2,1/2)}{B(1/2,1/2)}
=\frac{\binom{2n}{n}}{4^n}.
$$

For $n=0$ this is one; for $n=1,2$ it reproduces the values above. The [central binomial coefficient](central-binomial-coefficient.md) thus appears in an exact moment calculation for a continuous [probability distribution](probability-distribution-split.md).

## ↑ Ancestors (8)

1. [Arcsine distribution](arcsine-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
