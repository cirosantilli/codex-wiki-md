<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $u$ as a spectroscopic [wavenumber](../../../../wavenumber.md), in the same units throughout. Write the mass [absorption coefficient](../../../../absorption-coefficient.md) of the absorbing species as

$$
\boxed{\kappa_\nu=S\phi(\nu-\nu_0),\qquad
\int_{-\infty}^{\infty}\phi(\delta\nu)\,d\delta\nu=1,\qquad
S=\int\kappa_\nu\,d\nu.}
$$

Here $S$ is the [spectral line strength](../../../../spectral-line-strength.md), the integrated mass [absorption coefficient](../../../../absorption-coefficient.md); it is not the line-centre coefficient. If $\kappa_\nu$ has units $\mathrm{m^2\,kg^{-1}}$ and $\nu$ is in $\mathrm{cm^{-1}}$, then $S$ has units $\mathrm{m^2\,kg^{-1}\,cm^{-1}}$. For absorber [mass density](../../../../density.md) $\rho_a$, the volume coefficient in [Beer-Lambert law](../../../../beer-lambert-law.md) is $\rho_a\kappa_\nu$.

**[Lifetime broadening](../../../../lifetime-broadening.md).** Finite lifetimes of the upper and lower states destroy optical coherence, even for an isolated molecule. Exponential coherence decay gives a [Lorentzian line shape](../../../../lorentzian-line-shape.md). For population decay rates $\Gamma_u,\Gamma_l$ and no extra dephasing, its [wavenumber](../../../../wavenumber.md) half-width is $(\Gamma_u+\Gamma_l)/(4\pi c)$, with $c$ expressed in the length unit reciprocal to $\nu$. This sets a natural linewidth and can matter at extremely low collision rates; it is generally much smaller than atmospheric collisional or thermal widths.

**[Thermal Doppler broadening](../../../../thermal-doppler-broadening.md).** A [Maxwell-Boltzmann distribution](../../../../maxwell-boltzmann-distribution.md) of molecular line-of-sight velocities gives

$$
\phi_D(\delta\nu)=\frac{e^{-(\delta\nu/\Delta_D)^2}}{\sqrt\pi\Delta_D},\qquad
\Delta_D=\frac{\nu_0}{c}\sqrt{\frac{2k_BT}{m_a}}.
$$

This [Gaussian distribution](../../../../normal-distribution.md) has a $1/e$ half-width $\Delta_D$, determined by absorber [molecular mass](../../../../molecular-mass.md) $m_a$ and [temperature](../../../../temperature-split.md). It is especially relevant in the rarefied upper atmosphere, where collisions are infrequent.

**[Pressure broadening](../../../../pressure-broadening.md).** Collisions perturb transition [frequencies](../../../../frequency.md) and phases. In the impact regime, exponential phase decorrelation gives

$$
\phi_L(\delta\nu)=\frac1\pi\frac{\Delta_L}{\delta\nu^2+\Delta_L^2}.
$$

Here $\Delta_L$ is the half-width at half maximum, proportional to the coherence-destroying collision rate. It depends on perturber [density](../../../../density.md), molecular collision properties, and [temperature](../../../../temperature-split.md); it is often parameterized by $\Delta_L\propto p(T_*/T)^{n_T}$ for a specified broadener. It dominates much of the dense lower atmosphere. The [Lorentzian line shape](../../../../lorentzian-line-shape.md) has algebraic $\delta\nu^{-2}$ wings, whereas the [Doppler profile](../../../../thermal-doppler-broadening.md) has rapidly decreasing [Gaussian](../../../../normal-distribution.md) wings. Where both mechanisms matter, their convolution is a [Voigt profile](../../../../voigt-profile.md). A pure pressure-broadened profile should not be extrapolated to arbitrarily low [pressure](../../../../pressure-split.md) while discarding the finite Doppler core.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
