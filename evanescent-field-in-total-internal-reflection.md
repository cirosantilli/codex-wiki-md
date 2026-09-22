# Evanescent field in total internal reflection

↑ **Parent:** [Total internal reflection](total-internal-reflection.md)

The [evanescent field in total internal reflection](evanescent-field-in-total-internal-reflection.md) oscillates and advances in [wave phase](phase-waves.md) along the boundary while its [wave amplitude](wave-amplitude.md) decays away from it. With the coordinates above and time dependence $e^{-i\omega t}$, a [TE polarization](transverse-electric-polarization.md) has [complex amplitude](complex-amplitude.md)

$$
\mathbf E(x,z)=A e^{iqx-\kappa z}\widehat{\mathbf y},\qquad
\kappa=k_0\sqrt{n_1^2\sin^2\theta-n_2^2},\qquad \theta>\theta_c.
$$

The physical [electric field](electric-field-split.md) is $\operatorname{Re}[\mathbf E(x,z)e^{-i\omega t}]$. The decaying sign excludes a field that grows without bound at $z\to\infty$. [Dielectric-interface boundary conditions](dielectric-interface-boundary-conditions.md) determine $A$; for nongrazing incidence it is generally nonzero.[Total Internal Reflection and Evanescent Waves, equations (154)–(158), decaying sign and parallel energy flow](interactive-optics-by-sander-konijnenberg-aurele-j-l-adam-and-h-paul-urbach.md)

Zero normal [energy flux](energy-flux.md) follows directly from [Maxwell equations](maxwell-equations-split.md). The [wavevector](wavevector.md) is $(q,0,i\kappa)$; the relation $\mathbf H=(\mathbf k\times\mathbf E)/(\omega\mu_0)$ gives

$$
H_x=-\frac{i\kappa}{\omega\mu_0}E_y,\qquad H_z=\frac{q}{\omega\mu_0}E_y.
$$

Consequently, the cycle-averaged [Poynting vector](poynting-vector.md) is

$$
\langle\mathbf S\rangle=\frac12\operatorname{Re}(\mathbf E\times\mathbf H^*)
=\frac{q|A|^2}{2\omega\mu_0}e^{-2\kappa z}\widehat{\mathbf x},\qquad \langle S_z\rangle=0.
$$

The [electric field](electric-field-split.md) and $H_x$ are a quarter-cycle apart, so their product has zero cycle average. Tangential [energy flux](energy-flux.md) survives. This is a local calculation for the single decaying [evanescent wave](evanescent-wave.md) in the infinite second [half-space](half-space.md).

To check reflected [power](power.md) independently, put $a=n_1k_0\cos\theta>0$. The existing [transverse-electric Fresnel reflection coefficient](transverse-electric-fresnel-reflection-coefficient.md) becomes $r=(a-i\kappa)/(a+i\kappa)$. Its numerator and denominator are [complex conjugates](complex-conjugate.md), so $|r|^2=1$, while $1+r=2a/(a+i\kappa)\ne0$ supplies the surface [electric field](electric-field-split.md) relative to the incident [wave amplitude](wave-amplitude.md). Thus a unit [optical reflectance](reflectance.md) does not require a zero transmitted field. The same normal [power](power.md) balance holds for [TM polarization](transverse-magnetic-polarization.md); its reflected [wave phase](phase-waves.md) generally differs from the [TE polarization](transverse-electric-polarization.md) phase. A mixture can therefore change its [polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md) on reflection even though all normal incident [power](power.md) returns.

**Table of contents**

- [Evanescent penetration depth](evanescent-penetration-depth.md)

## ↑ Ancestors (11)

1. [Total internal reflection](total-internal-reflection.md)
2. [Snell law for electromagnetic waves](snell-law-for-electromagnetic-waves.md)
3. [Phase matching at a planar wave interface](phase-matching-at-a-planar-wave-interface.md)
4. [Dielectric-interface boundary conditions](dielectric-interface-boundary-conditions.md)
5. [Interface conditions for electromagnetic fields](interface-conditions-for-electromagnetic-fields.md)
6. [Plane electromagnetic wave](plane-electromagnetic-wave.md)
7. [Electromagnetic wave](electromagnetic-wave-split.md)
8. [Electromagnetism](electromagnetism-split.md)
9. [Branches of physics](branches-of-physics.md)
10. [Physics](physics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Evanescent field in total internal reflection](evanescent-field-in-total-internal-reflection.md)
- [Frustrated total internal reflection](frustrated-total-internal-reflection.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2/section-b/b7/d/solution.md)
- [Total internal reflection](total-internal-reflection.md)
