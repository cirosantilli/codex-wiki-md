<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [single-line greenhouse deficit](../../../../single-line-greenhouse-deficit.md), use [hydrostatic balance](../../../../hydrostatic-balance.md), fixed [surface pressure](../../../../pressure-split.md) $p_s$, constant [gravity](../../../../gravity.md) $g$, and the [dry adiabat](../../../../dry-adiabat.md)

$$
T(p)=T_s(p/p_s)^\kappa,\qquad \kappa=R_b/c_{p,b}>0.
$$

The gas constant and [specific heat](../../../../specific-heat-capacity.md) refer to the background gas. Let $\mu_d=\cos\tilde\theta>0$ be the supplied effective ray cosine. The vertical [optical depth](../../../../optical-depth.md) and slant [transmittance](../../../../transmittance.md) from level $p$ to space are

$$
\tau_\nu(p)=\frac qg\int_0^p\kappa_\nu(p',T(p'))\,dp',\qquad
\mathfrak T_\nu(p)=\exp[-\tau_\nu(p)/\mu_d].
$$

This permits pressure-dependent [line widths](../../../../spectral-line-broadening.md). With [local thermodynamic equilibrium](../../../../local-thermodynamic-equilibrium.md), negligible infrared [scattering](../../../../scattering.md), a black thermal surface, and no incident [thermal radiation](../../../../thermal-radiation.md) from space, the formal [radiative transfer](../../../../radiative-transfer.md) solution is

$$
I_\nu(0)=B_\nu(T_s)\mathfrak T_\nu(p_s)+
\int_0^{p_s}B_\nu(T(p))[-\partial_p\mathfrak T_\nu(p)]\,dp.
$$

The weights add to one. Subtract the transparent-surface [radiance](../../../../radiance.md) and put $B(p)=B_{\nu_0}(T(p))$, using the narrow-line approximation only in the line deficit. Define its pressure-dependent [equivalent width](../../../../equivalent-width.md)

$$
E(p,q)=\int[1-\mathfrak T_\nu(p)]\,d\nu,\qquad
\partial_pE=\int\frac{q\kappa_\nu(p)}{g\mu_d}\mathfrak T_\nu(p)\,d\nu\ge0.
$$

Approximating each hemispheric flux by $\pi$ times the effective-ray [radiance](../../../../radiance.md) preserves the black-surface flux. The outgoing longwave flux is therefore

$$
F_{\rm out}=\sigma_{\rm SB}T_s^4-D(T_s,q),\qquad
\boxed{D=\pi\int_0^{p_s}[B(p_s)-B(p)]\,\partial_pE(p,q)\,dp.}
$$

Integration by parts gives the particularly transparent form

$$
\boxed{D=\pi\int_0^{p_s}E(p,q)\frac{dB(p)}{dp}\,dp\ge0.}
$$

Both boundary terms vanish: $E(0,q)=0$ and $B(p_s)-B(p_s)=0$. The [dry adiabat](../../../../dry-adiabat.md) and monotonic [Planck function](../../../../planck-function.md) give $dB/dp>0$. Atmospheric emission replaces part of the warm surface radiation by emission from cooler levels, reducing emission to space for a specified $T_s$. The inequality is strict when [opacity](../../../../opacity.md) occurs over a nonzero range with [temperature](../../../../temperature-split.md) contrast; an [isothermal](../../../../isothermal-process.md) absorbing layer at the surface [temperature](../../../../temperature-split.md) would not produce such a contrast.

For a spherical [planet](../../../../planet.md) the mean absorbed instellation is $F_*=(1-\alpha)L_{\circledast}/4$. The required global [energy balance](../../../../energy-balance.md) is

$$
\boxed{\sigma_{\rm SB}T_s^4=\frac{(1-\alpha)L_{\circledast}}4+D(T_s,q).}
$$

Consequently every equilibrium of this model has $T_s\ge T_{\rm bare}=[(1-\alpha)L_{\circledast}/(4\sigma_{\rm SB})]^{1/4}$, with strict warming when $D>0$. At fixed [temperature profile](../../../../temperature-split.md), increasing $q$ increases $E$ and hence $D$. This argument does not assume that the greenhouse gas changes the stellar-band [albedo](../../../../albedo.md), [surface pressure](../../../../pressure-split.md), or background thermodynamics; those are held fixed. For sufficiently broad or overlapping saturated wings the full frequency-dependent [Planck function](../../../../planck-function.md) must replace the narrow-line approximation.

## ↑ Ancestors (12)

1. [C](../c.md)
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
