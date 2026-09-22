<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [Brownian motion](../../../../brownian-motion-split.md) displacement has a [normal distribution](../../../../normal-distribution.md) with [variance](../../../../variance-split.md) $\Gamma t$. Its transition [probability density function](../../../../probability-density-function.md) is therefore

$$
p(y_f,t\mid y_i,0)
=\frac1{\sqrt{2\pi\Gamma t}}
\exp\!\left[-\frac{(y_f-y_i)^2}{2\Gamma t}\right].
$$

Comparison with the [free particle](../../../../free-particle.md) [heat kernel](../../../../heat-kernel.md) obtained in part (c) gives the required matching:

$$
\boxed{\Gamma t=\frac{\beta\hbar^2}{m}.}
$$

This matches whole path distributions after a linear reparametrization, not merely endpoint [variances](../../../../variance-split.md). To see this, divide the Brownian duration $t$ into $M$ slices of size $\delta t$. The [independent increments](../../../../independent-increments.md) have [normal distributions](../../../../normal-distribution.md) with [variance](../../../../variance-split.md) $\Gamma\delta t$, so their joint density contributes

$$
\prod_{j=1}^M\frac1{\sqrt{2\pi\Gamma\delta t}}
\exp\!\left[-\sum_{j=1}^M\frac{(y_j-y_{j-1})^2}{2\Gamma\delta t}\right].
$$

For the [Euclidean path integral](../../../../euclidean-path-integral.md), the corresponding expression is

$$
\prod_{j=1}^M\sqrt{\frac{m}{2\pi\hbar\delta\tau}}
\exp\!\left[-\sum_{j=1}^M\frac{m(x_j-x_{j-1})^2}{2\hbar\delta\tau}\right],
\qquad \delta\tau=\frac{\beta\hbar}{M}.
$$

The matching condition makes $\Gamma\delta t=\hbar\delta\tau/m$, so both the exponents and all normalization factors coincide. In particular, identifying Brownian time with [imaginary time](../../../../imaginary-time.md), $t=\beta\hbar$, requires $\Gamma=\hbar/m$, or [diffusion coefficient](../../../../diffusion-coefficient.md) $D=\hbar/(2m)$.

With both endpoints fixed, the normalized path law is a **[Brownian bridge](../../../../brownian-bridge.md)**. The [Euclidean path integral](../../../../euclidean-path-integral.md) itself is the endpoint density times that conditional path law. In the normalized time coordinate $s=\tau/(\beta\hbar)$, its [expected value](../../../../expected-value-split.md) and [covariance](../../../../covariance.md) are

$$
\mathbb E[x(s)]=x_i+s(x_f-x_i),
\qquad
\operatorname{Cov}(x(s),x(s'))
=\frac{\beta\hbar^2}{m}\bigl[\min(s,s')-ss'\bigr].
$$

The [classical path](../../../../classical-path.md) is therefore the bridge's [expected value](../../../../expected-value-split.md), while individual [Brownian bridge](../../../../brownian-bridge.md) paths fluctuate about it. Typical [Brownian motion](../../../../brownian-motion-split.md) paths are continuous but nowhere differentiable: the kinetic [Euclidean action](../../../../euclidean-action.md) is interpreted through the [time-sliced diffusion path integral](../../../../time-sliced-diffusion-path-integral.md), rather than by assuming that a typical path has an ordinary velocity.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the field theories and collective phenomena in condensed matter course of the University of Oxford](../../../split.md)
5. [Field theories and collective phenomena in condensed matter course of the University of Oxford](../../../../field-theories-and-collective-phenomena-in-condensed-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
