<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $D(0)=1$. The [present-extrapolated spherical-collapse barrier](../../../../../../present-extrapolated-spherical-collapse-barrier.md) is $\delta_c(z)=\delta_{\rm sc}/D(z)$, where $\delta_{\rm sc}\simeq1.686$ is the linear contrast extrapolated to spherical collapse in a matter-dominated universe. It is not the nonlinear interior overdensity $18\pi^2$. The [cosmological mass variance](../../../../../../smoothed-matter-density-variance.md) $\sigma^2(M,0)$ is the variance of the present-extrapolated linear [density contrast](../../../../../../density-contrast.md) smoothed over a mass $M$. It is not the variance of already virialized halo densities.

For a fixed-shape smoothing filter and $P(k)=P_0k^n$, rescale the variance integral with $x=kR$:

$$
\sigma^2(R)=\frac{P_0}{2\pi^2}R^{-(n+3)}\int_0^\infty x^{n+2}|W(x)|^2dx.
$$

Thus $\sigma(M,0)=S M^{-q}$, with $q=(n+3)/6$ and $S$ a normalization carrying the appropriate mass units. For a real-space [top-hat filter](../../../../../../top-hat-filter.md), convergence requires $-3<n<1$; a spectrum outside this interval needs physical cutoffs and does not have this unrestricted scale-free result.

If $n(M,z)dM$ counts halos per comoving volume, the [Press-Schechter halo mass function](../../../../../../press-schechter-halo-mass-function.md) follows by differentiating the cumulative mass fraction and converting mass fraction to number:

$$
n(M,z)=-\frac{\bar\rho_{m,0}}M\frac{\partial f(>M,z)}{\partial M}
=\sqrt{\frac2\pi}\frac{\bar\rho_{m,0}}{M^2}q\nu e^{-\nu^2/2},\qquad
\nu=\frac{\delta_c(z)}{\sigma(M,0)}.
$$

The minus sign is needed because the cumulative fraction decreases with $M$. To match the printed exponential coefficient exactly, define $M_*(z)$ by

$$
\frac{\nu^2}{2}=\left(\frac M{M_*}\right)^{2q},\qquad
\boxed{\sigma(M_*,0)=\frac{\delta_c(z)}{\sqrt2}.}
$$

This [peak-height calibration from an exponential mass-function cutoff](../../../../../../peak-height-calibration-from-an-exponential-mass-function-cutoff.md) differs from the also-common convention $\nu(M_*)=1$. Here $\nu=\sqrt2(M/M_*)^q$, and consequently

$$
\boxed{\alpha=q-2=\frac{n-9}{6},\quad\beta=2q=\frac{n+3}{3},\quad
A(z)=\frac{2q}{\sqrt\pi}\bar\rho_{m,0}M_*^{-q}
=\frac{n+3}{3\sqrt\pi}\bar\rho_{m,0}M_*^{-(n+3)/6}.}
$$

Equivalently $A=\sqrt{2/\pi}\,q\bar\rho_{m,0}\delta_c/S$. The [scale-free halo cutoff normalization](../../../../../../scale-free-halo-cutoff-normalization.md) therefore evolves with $z$; the displayed $A$ is not a redshift-independent universal constant. For physical number density, replace $\bar\rho_{m,0}$ by $\bar\rho_m(z)$ instead. Since $M_*=(\sqrt2S/\delta_c)^{1/q}$, it grows as $D^{6/(n+3)}$; in matter domination it is proportional to $(1+z)^{-6/(n+3)}$. At the collapse epoch itself, $\sigma(M_*,z)=\delta_{\rm sc}/\sqrt2$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
