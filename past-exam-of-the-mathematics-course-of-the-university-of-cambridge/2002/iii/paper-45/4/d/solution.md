<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Press-Schechter formalism](../../../../../../press-schechter-formalism.md) starts from a statistically homogeneous Gaussian initial [density contrast](../../../../../../density-contrast.md) with variance specified by its linear [matter power spectrum](../../../../../../matter-power-spectrum.md). Average it on mass scale $M=(4\pi/3)\bar\rho_{m0}R^3$, usually with a spherical top-hat. Let $\sigma(M,t)=b(t)\sigma_0(M)$, normalizing $b$ consistently. Assume that a region becomes a collapsed halo when its linearly extrapolated smoothed density exceeds a mass-independent [linear spherical-collapse threshold](../../../../../../linear-spherical-collapse-threshold.md) $\delta_{
m sc}\simeq1.686$ in the Einstein-de Sitter approximation. This extrapolates a linear Gaussian statistic to a nonlinear collapse criterion, and ignores the detailed nonspherical dynamics.

The one-scale Gaussian upper tail only assigns half the mass to overdense regions when the variance grows without limit. The conventional factor of two is inserted to account for material in larger collapsed regions even if it falls below the threshold on a smaller scale, the cloud-in-cloud issue. A first-crossing excursion-set argument can justify that factor for an ideal sharp-k filter; it is not a theorem that an arbitrary top-hat one-scale probability alone supplies it. With this prescription, the mass fraction in objects above $M$ is

$$
F(>M,t)=\operatorname{erfc}\left(\frac{\delta_{
m sc}}{\sqrt2\,\sigma(M,t)}\right).
$$

Convert mass fraction to comoving number density by assigning mass $M$ to each halo, using $dn/dM=(\bar\rho_{m0}/M)|dF/dM|$. This yields the [Press-Schechter halo mass function](../../../../../../press-schechter-halo-mass-function.md)

$$
\boxed{\frac{dn}{dM}=\sqrt{\frac2\pi}\frac{\bar\rho_{m0}}{M^2}\,
\nu\left|\frac{d\ln\sigma}{d\ln M}\right|e^{-\nu^2/2},\qquad
\nu=\frac{\delta_{
m sc}}{b(t)\sigma_0(M)}.}
$$

Equivalently one can use a present-extrapolated threshold $\delta_c(t)=\delta_{
m sc}/b(t)$ and present variance; using both that threshold and an already grown variance would double-count growth. The model assumes approximate mass conservation, a smoothing-to-halo-mass assignment and a spherical universal barrier. It is an approximation to gravitational halo formation, not an exact partition of the real cosmic web.

In hierarchical formation, $\sigma_0(M)$ decreases with mass: smaller regions become nonlinear first and are subsequently incorporated into larger haloes. Define a characteristic mass by $b(t)\sigma_0(M_*)=\delta_{
m sc}$. It increases as growth proceeds, moving the exponential cutoff towards larger masses. For a scale-free spectrum with well-defined top-hat variance, $-3<n<1$, $\sigma_0\propto M^{-(n+3)/6}$ and hence $M_*\propto b^{6/(n+3)}$. At a fixed mass, the derivative of $\ln(dn/dM)$ with respect to $\ln b$ is $\nu^2-1$: rare high-mass abundances grow, while the small-mass abundance can decline as objects merge into larger systems. Thus one must not claim that every fixed-mass bin increases forever. The growth of $M_*$ is the [scale-free characteristic mass in the Press-Schechter formalism](../../../../../../scale-free-characteristic-mass-in-the-press-schechter-formalism.md).

For the temperature test, [virial equilibrium](../../../../../../virial-equilibrium.md) and gas [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) give $k_BT\sim\mu m_pGM/R$. Defining the halo radius by $M=(4\pi/3)\Delta_v\rho_c(z)R^3$ yields

$$
T\propto M^{2/3}[\Delta_v\rho_c(z)]^{1/3}.
$$

A calibrated monotone mass-temperature relation converts the mass function to $dn/dT=(dn/dM)|dM/dT|$, with temperature scatter treated by convolution when necessary. The [cluster temperature function normalization](../../../../../../cluster-temperature-function-normalization.md) is strongly sensitive to the linear fluctuation amplitude: at fixed mass and spectral shape, $\partial\ln n/\partial\ln\sigma_8=\nu^2-1$. Rare hot clusters occupy the exponential tail, so even a modest amplitude change can produce a large abundance change. Here [sigma eight](../../../../../../eight-megaparsec-density-fluctuation-amplitude.md) is the rms linear density contrast today in an $8h^{-1}\,\mathrm{Mpc}$ top-hat, not the full spectrum.

Compare observed cluster-temperature counts and their redshift evolution with these predictions to constrain that normalization jointly with matter density and growth. The mass-temperature calibration, selection volume, temperature scatter, nonthermal support and deviations from the ideal halo mass function limit a temperature-only inference. **The abundance of rare hot clusters is a sensitive amplitude probe once their mass calibration and cosmology are specified.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
