<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $D(z)$ be the [linear growth factor](../../../../../../linear-growth-factor.md) normalized to $D(0)=1$. The [present-extrapolated spherical-collapse barrier](../../../../../../present-extrapolated-spherical-collapse-barrier.md) is $\delta_c(z)=\delta_{\rm sc}/D(z)$, where $\delta_{\rm sc}\simeq1.686$ is the linearly evolved overdensity required for spherical collapse at that epoch. The [smoothed matter density variance](../../../../../../smoothed-matter-density-variance.md) $\sigma(M,z)$ is the root-mean-square linear [density contrast](../../../../../../density-contrast.md) after smoothing on a Lagrangian region containing mass $M$; $\sigma(M,z)=D(z)\sigma(M,0)$. Thus the barrier-to-variance ratio is equivalently $\delta_c(z)/\sigma(M,0)=\delta_{\rm sc}/\sigma(M,z)$.

For a [spherical top-hat window function](../../../../../../spherical-top-hat-window-function.md) with comoving radius $R$, $M=(4\pi/3)\bar\rho_{m,0}R^3$. A scale-free spectrum gives

$$
\sigma^2(M,z)\propto D^2(z)\int_0^\infty k^{n+2}|W(kR)|^2\,dk\propto D^2(z)R^{-(n+3)}.
$$

Changing variable to $kR$ gives the [scale-free smoothed density variance](../../../../../../scale-free-smoothed-density-variance.md) scaling $\sigma\propto M^{-\beta}$ with $\beta=(n+3)/6$. For a top-hat the scale-free integral converges for $-3<n<1$; the inferred index below lies in this interval.

Differentiate the [Press-Schechter formalism](../../../../../../press-schechter-formalism.md) mass fraction and divide the resulting mass density by halo mass. Writing $\nu=\delta_{\rm sc}/\sigma(M,z)$,

$$
\frac{dn_h}{dM}=\frac{\bar\rho_{m,0}}{M}\left|\frac{df(>M)}{dM}\right|=\sqrt{\frac2\pi}\frac{\bar\rho_{m,0}}{M^2}\,\beta\nu\,e^{-\nu^2/2}.
$$

This is a comoving halo abundance. Introduce $M_{h,\rm ch}$ by $\nu^2/2=(M/M_{h,\rm ch})^{2\beta}$; then $\sigma(M_{h,\rm ch},z)=\delta_{\rm sc}/\sqrt2$ and

$$
\frac{dn_h}{dM}=\frac{2\beta}{\sqrt\pi}\frac{\bar\rho_{m,0}}{M_{h,\rm ch}^2}\left(\frac{M}{M_{h,\rm ch}}\right)^{\beta-2}e^{-(M/M_{h,\rm ch})^{2\beta}}.
$$

For the [constant baryon conversion mapping of halo and stellar mass](../../../../../../constant-baryon-conversion-mapping-of-halo-and-stellar-mass.md), identify one counted galaxy with each halo and neglect scatter and subhalo multiplicity. If $f_*$ is the fraction of the halo's baryons incorporated into stars, its [stellar-to-halo mass ratio](../../../../../../stellar-to-halo-mass-ratio.md) is $\epsilon_*=f_*f_b$, with $f_b=0.2$, and $M_*=\epsilon_*M$. The corresponding stellar characteristic mass is $M_{*,\rm ch}=\epsilon_*M_{h,\rm ch}$. Transforming $dn_h/dM$ with $dM/dM_*=1/\epsilon_*$ gives the [power-law Press-Schechter stellar mass function](../../../../../../power-law-press-schechter-stellar-mass-function.md):

$$
\boxed{\frac{dn_*}{dM_*}=\frac{2\beta}{\sqrt\pi}\frac{\bar\rho_{m,0}\epsilon_*}{M_{*,\rm ch}^2}\left(\frac{M_*}{M_{*,\rm ch}}\right)^{\beta-2}\exp\left[-\left(\frac{M_*}{M_{*,\rm ch}}\right)^{2\beta}\right].}
$$

It has the required power-law low-mass behavior and stretched exponential cutoff. Matching both exponents and the normalization determines the effective spectral index and stellar conversion efficiency.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
