<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a closed absorbing [two-level system](../../../../two-level-system.md), write $N=N_1+N_2$, let $A=1/\tau$, and use $\sigma_a=\sigma_{12}$ for the [absorption cross section](../../../../absorption-cross-section.md). This differs from the stimulated-[emission cross section](../../../../emission-cross-section.md) convention in part (a). With $r=g_2/g_1$, the [rate equations](../../../../rate-equation.md) are

$$
\boxed{\dot N_2=\frac{\sigma_a I}{\hbar\omega}\left(N_1-\frac{N_2}{r}\right)-AN_2,\qquad
\dot N_1=-\dot N_2.}
$$

At steady state, $N_2=W_aN/[A+(1+1/r)W_a]$ for $W_a=\sigma_aI/(\hbar\omega)$. Hence the positive [absorption coefficient](../../../../absorption-coefficient.md) is

$$
\kappa=\sigma_a\left(N_1-\frac{N_2}{r}\right)
=\frac{N\sigma_a}{1+I/I_{s,a}},\qquad
I_{s,a}=\frac{\hbar\omega}{(1+1/r)\sigma_a\tau}.
$$

For the given [sodium](../../../../sodium.md) fine-structure transition, the [statistical weights](../../../../statistical-weight.md) are $g_1=2$, $g_2=4$, so $r=2$ and $1+1/r=3/2$. The small-signal transmission gives the [optical depth](../../../../optical-depth.md)

$$
D_0=N\sigma_aL=-\ln0.90=0.1053605.
$$

To account for the finite decrease of [intensity](../../../../intensity-physics.md) through the sample, integrate $dI/dz=-\kappa I$ rather than treating the stronger beam as exactly uniform. If $T=I_{\rm out}/I_{\rm in}$, this gives

$$
\ln T+\frac{I_{\rm in}(T-1)}{I_{s,a}}=-D_0,\qquad
I_{s,a}=\frac{I_{\rm in}(1-T)}{D_0+\ln T}.
$$

Taking $270\,\mathrm{W\,m^{-2}}$ as the incident [intensity](../../../../intensity-physics.md) and $T=0.967$,

$$
I_{s,a}=\frac{270(0.033)}{0.1053605+\ln0.967}
\simeq124.09\,\mathrm{W\,m^{-2}}.
$$

Using the [photon energy](../../../../photon-energy.md) $hc/\lambda$ then gives

$$
\boxed{\sigma_a=\frac{hc}{(3/2)\lambda\tau I_{s,a}}
\simeq1.13\times10^{-13}\,\mathrm{m^2}.}
$$

Ignoring the small variation of the stronger [intensity](../../../../intensity-physics.md) would instead give about $1.11\times10^{-13}\,\mathrm{m^2}$; the integrated value uses the stated transmissions more consistently. The length is not needed to eliminate $N$, but gives the check $N\simeq9.3\times10^{14}\,\mathrm{m^{-3}}$.

The resonant [absorption cross section](../../../../absorption-cross-section.md) is of optical-[wavelength](../../../../wavelength.md)-squared size, much larger than a typical atomic geometric collision area. [Pressure broadening](../../../../pressure-broadening.md) [cross sections](../../../../cross-section-physics.md) involve phase-changing interatomic encounters and need not equal hard-sphere collision areas; their numerical value depends on collision partners and speed. No precise ratio follows from the supplied data. A useful distinction is that resonant [absorption](../../../../absorption-electromagnetic-radiation.md) involves coherent response on the optical scale, so its [cross section](../../../../cross-section-physics.md) need not resemble an [chemical atom](../../../../atom-physics.md)'s geometric area.

For [homogeneous spectral broadening](../../../../homogeneous-spectral-broadening.md), all participating [chemical atoms](../../../../atom-physics.md) must share the same [resonance](../../../../resonance.md) and single-atom response width. In a dilute sample dominated by [natural linewidth](../../../../natural-linewidth.md), the weak-beam requirement is

$$
\Delta\nu_D=\frac1\lambda\sqrt{\frac{8\ln2\,k_BT}{m_{\rm Na}}}
\ll\frac1{2\pi\tau}\simeq9.95\,\mathrm{MHz}.
$$

Using the [sodium](../../../../sodium.md) [atomic mass](../../../../atomic-mass.md), equality occurs near $T=0.017\,\mathrm K$, so $T\ll17\,\mathrm{mK}$ is a sufficient thermal condition. Spatial [Zeeman energy](../../../../zeeman-energy.md) shifts, light shifts and transit effects should also be small, the [laser](../../../../laser-split.md) should address the same selected component, and the interaction should last long enough for steady populations. Uniform impact [pressure broadening](../../../../pressure-broadening.md) can also be homogeneous, but would change the width and effective [cross section](../../../../cross-section-physics.md); it is not included in the lifetime-only numerical model.

Real [sodium](../../../../sodium.md) also has [hyperfine structure](../../../../hyperfine-structure.md) and [optical pumping](../../../../optical-pumping.md) among [magnetic sublevels](../../../../magnetic-sublevel.md). The inferred $\sigma_a$ is the effective cross section of the stated $g_J=2J+1$ [two-level system](../../../../two-level-system.md) model, assuming statistical sublevel populations and no loss into unaddressed states. A measurement on a resolved, polarized closed [hyperfine structure](../../../../hyperfine-structure.md) component requires its actual [transition dipole moment](../../../../electric-dipole-transition-moment.md) and [selection rules](../../../../selection-rule.md); a universal polarization-independent [sodium](../../../../sodium.md) cross section cannot be inferred from this simplified model. The dependence of resonant cross sections and [saturation intensities](../../../../saturation-intensity.md) on sublevel preparation is tabulated explicitly for the real [sodium](../../../../sodium.md) D lines.[Section on saturation intensity and resonant scattering cross section, and Table 7](../../../../sodium-d-line-data-by-daniel-a-steck.md)

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the atomic and laser physics course of the University of Oxford](../../../split.md)
5. [Atomic and laser physics course of the University of Oxford](../../../../atomic-and-laser-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
