<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

First take $z>0$. Set $s=t^3-1$ in the tail integral. This puts it in the endpoint form needed for [Watson's lemma](../../../../../watson-s-lemma.md):

$$
F(z)=\frac{e^{-z^3}}3\int_0^\infty e^{-z^3s}(1+s)^{-2/3}\,ds.
$$

The binomial coefficients are $(-1)^r(2/3)_r/r!$, where $(a)_r=\Gamma(a+r)/\Gamma(a)$ is the [rising factorial](../../../../../rising-factorial.md). Integrating each endpoint term gives

$$
\boxed{F(z)\sim\frac{e^{-z^3}}{3z^3}\sum_{r\geq0}\frac{(-1)^r\Gamma(r+2/3)}{\Gamma(2/3)z^{3r}}.}
$$

Also, scaling the complete positive-ray integral gives $\int_0^\infty e^{-z^3t^3}dt=\Gamma(1/3)/(3z)$. Hence

$$
\boxed{G(z)\sim\frac{\Gamma(1/3)}{3z}-\frac{e^{-z^3}}{3z^3}\left[1-\frac{2}{3z^3}+\frac{10}{9z^6}-\cdots\right].}
$$

The endpoint term is exponentially small on this positive ray but must be retained for continuation to other sectors.

For complex $z$, use $s=zt$ so $G(z)=z^{-1}\int_0^z e^{-s^3}ds$. Put $C=\Gamma(1/3)/3$ and $\omega=e^{2\pi i/3}$. The complete [steepest descent contours](../../../../../steepest-descent-contour.md) from the cubic saddle are the rays $\arg s=2\pi j/3$, whose integrals are $C\omega^j$. Deform the finite contour onto one of these rays followed by the endpoint contour. The [cubic exponential integral Stokes sectors](../../../../../cubic-exponential-integral-stokes-sectors.md) give

$$
\boxed{G(z)\sim\frac{C\omega^j}{z}-\frac{e^{-z^3}}{3z^3}\sum_{r\geq0}\frac{(-1)^r(2/3)_r}{z^{3r}},\qquad \frac{(2j-1)\pi}{3}<\arg z<\frac{(2j+1)\pi}{3}.}
$$

For $0\leq\arg z\leq2\pi$, take $j=0$ below $\pi/3$, $j=1$ between $\pi/3$ and $\pi$, $j=2$ between $\pi$ and $5\pi/3$, and $j=3$ above $5\pi/3$. The corresponding algebraic coefficients are $C,C\omega,C\omega^2,C$. A negative-real $z$ provides a useful sign check: $G(z)=G(|z|e^{i\pi})$ is real and positive, so its two lateral algebraic coefficients must be [complex conjugates](../../../../../complex-conjugate.md).

The subdominant algebraic term switches across the [Stokes lines](../../../../../stokes-line.md)

$$
\boxed{\arg z=\frac\pi3,\ \pi,\ \frac{5\pi}3.}
$$

There $z^3$ is negative real and the endpoint exponential is dominant. The intervening [anti-Stokes lines](../../../../../anti-stokes-line.md) are $\arg z=\pi/6+j\pi/3$, where $\operatorname{Re}z^3=0$ and the exponential changes from growth to decay. The naming convention here distinguishes switching from equal exponential magnitude.

To resolve the jump near $\theta_s=\pi/3$, optimally truncate the endpoint series at $N$ with $N+2/3=R+O(1)$, where $R=|z|^3$. Let $P_N$ denote that truncated endpoint contribution. The [Borel remainder for a cubic exponential integral](../../../../../borel-remainder-for-a-cubic-exponential-integral.md) derived in [solution](a/solution.md), together with the [Gaussian pole transition for a large gamma parameter](../../../../../gaussian-pole-transition-for-a-large-gamma-parameter.md) in [solution](b/solution.md), gives

$$
\boxed{G(z)=P_N(z)+\frac C z\left[1+(\omega-1)S(\theta)\right]+O\left(\frac1{|z|\sqrt R}\right),\qquad S(\theta)=\frac12\left[1+\operatorname{erf}\left(3(\theta-\pi/3)\sqrt{\frac R2}\right)\right].}
$$

This estimate is on the transition scale $\theta-\pi/3=O(R^{-1/2})$ after [optimal truncation](../../../../../optimal-truncation.md). The [error-function smoothing of a Stokes multiplier](../../../../../error-function-smoothing-of-a-stokes-multiplier.md) has width $O(|z|^{-3/2})$. Before the line $S\to0$ and the coefficient is $C$; after it $S\to1$ and the coefficient is $C\omega$, agreeing with the sector expansions. On the line the leading coefficient is their average. The original $G$ is an [entire function](../../../../../entire-function.md); only its asymptotic decomposition has these sector-dependent coefficients.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 79](../../paper-79-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

## ← Incoming links (1)

- [Solution](b/solution.md)
