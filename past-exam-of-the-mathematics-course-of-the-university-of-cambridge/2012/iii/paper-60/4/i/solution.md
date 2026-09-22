<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\delta_{\rm sc}\simeq1.686$ be the [linear spherical-collapse threshold](../../../../../../linear-spherical-collapse-threshold.md) and let $D(t)$ be the [linear growth factor](../../../../../../linear-growth-factor.md), normalized to one at the epoch to which the random density field has been extrapolated. The time-dependent barrier is $\delta_c(t)=\delta_{\rm sc}/D(t)$. The [smoothed matter density variance](../../../../../../smoothed-matter-density-variance.md) $\sigma^2(M)$ is the variance of the linear [density contrast](../../../../../../density-contrast.md) smoothed with a [spherical top-hat window function](../../../../../../spherical-top-hat-window-function.md) whose comoving mass is $M$. Both quantities must refer to the same linear normalization; equivalently use $\nu=\delta_{\rm sc}/\sigma(M,t)$.

Let $N$ denote the comoving number density and write $\mathcal N(M,t)=dN/dM$ for the positive differential [Press-Schechter halo mass function](../../../../../../press-schechter-halo-mass-function.md). With $\bar\rho_0$ the mean comoving mass density, the mass fraction obeys

$$
f(>M,t)=\frac1{\bar\rho_0}\int_M^\infty M'\mathcal N(M',t)\,dM',\qquad \mathcal N(M,t)=-\frac{\bar\rho_0}M\frac{\partial f}{\partial M}.
$$

Differentiating the [complementary error function](../../../../../../complementary-error-function.md) and using $\nu=\delta_c/\sigma$ gives

$$
\boxed{\frac{dN}{dM}=\sqrt{\frac2\pi}\frac{\bar\rho_0}{M^2}\nu e^{-\nu^2/2}\left|\frac{d\ln\sigma}{d\ln M}\right|.}
$$

This is the requested mass function; $M\,dN/dM$ is the abundance per unit natural logarithmic mass. For physical rather than [comoving number density](../../../../../../comoving-number-density.md), multiply by $(1+z)^3$. The normalization in the [Press-Schechter formalism](../../../../../../press-schechter-formalism.md) includes its factor of two relative to the positive Gaussian tail, so $f(>M)$ tends to one as the smoothing mass tends to zero when $\sigma$ diverges. It is a collapse prescription, not the probability that an arbitrary already nonlinear density field stays Gaussian.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
