# Waveguide cutoff frequency

↑ **Parent:** [Rectangular electromagnetic waveguide](rectangular-electromagnetic-waveguide.md)

The [waveguide cutoff frequency](waveguide-cutoff-frequency.md) separates oscillatory axial propagation from [exponential decay](exponential-decay.md) for a particular [normal mode](normal-mode.md). For the [vacuum](vacuum.md)-filled [rectangular electromagnetic waveguide](rectangular-electromagnetic-waveguide.md), the [dispersion relation](dispersion-relation-split.md) is

$$
\kappa_{mn}^2=\left(\frac{m\pi}{a}\right)^2+\left(\frac{n\pi}{b}\right)^2,\qquad
\omega_{mn}=c\kappa_{mn},\qquad
\beta^2=\frac{\omega^2-\omega_{mn}^2}{c^2}.
$$

For a [transverse electric mode of a rectangular waveguide](transverse-electric-mode-of-a-rectangular-waveguide.md), $m,n$ are nonnegative [integers](integer-split.md) but not both zero. For a mode with $B_z=0$ and nonzero $E_z$, both indices must be positive. The lowest cutoff for $a>b$ is consequently $\omega_{10}=\pi c/a$, or ordinary [frequency](frequency.md) $f_c=c/(2a)$.

A square cross-section instead gives equal $\mathrm{TE}_{10}$ and $\mathrm{TE}_{01}$ cutoffs. The absence of a [transverse electromagnetic mode](transverse-electromagnetic-mode.md) is specific to this hollow pipe, rather than all [electromagnetic waveguides](electromagnetic-waveguide.md).[Haus and Melcher, Electromagnetic Fields and Energy, §13.4, equations (26)–(27) and Fig. 13.4.3: allowed indices, dominant mode and square-guide degeneracy](electromagnetic-fields-and-energy-by-hermann-a-haus-and-james-r-melcher/rectangular-waveguide-modes.md)

For $\omega>\omega_{mn}$, choose real $\beta>0$ for propagation toward $+z$. For $0<\omega<\omega_{mn}$, a field decaying into a semi-infinite guide has

$$
\beta=i\alpha,\qquad \alpha=\frac{\sqrt{\omega_{mn}^2-\omega^2}}{c}>0,\qquad e^{i\beta z}=e^{-\alpha z}.
$$

A finite section can contain both growing and decaying axial solutions set by its two ends; the single decaying solution is not a complete finite-section transmission calculation. At exact cutoff $\beta=0$, the two axial solutions become a constant and a linear function of $z$: there is no finite axial [wavelength](wavelength.md) for a traveling sinusoid.

In the chosen $a=30\,\mathrm{mm}$ guide at $f=0.8f_c=3.99723277\,\mathrm{GHz}$, the $\mathrm{TE}_{10}$ branch has $\alpha=20\pi\,\mathrm{m}^{-1}$. Its amplitude decay length is $1/\alpha\simeq15.9155\,\mathrm{mm}$; after $50\,\mathrm{mm}$, its normalized [wave amplitude](wave-amplitude.md) is $e^{-\pi}\simeq0.0432139$. This is geometric evanescence even with ideal walls, not [Joule heating](joule-heating.md). A single decaying branch has zero cycle-averaged axial [Poynting vector](poynting-vector.md): substituting $\beta=i\alpha$ makes $B_x$ a quarter-cycle out of phase with $E_y$. Coupling across a finite section requires the complete boundary-value solution.

<a id="image-original-te10-model-propagating-dispersion-above-cutoff-and-spatial-amplitude-decay-below-cutoff"></a>
![](rectangular-waveguide-cutoff-and-dispersion.png)

**[Figure 3](#image-original-te10-model-propagating-dispersion-above-cutoff-and-spatial-amplitude-decay-below-cutoff). Original TE10 model: propagating dispersion above cutoff and spatial amplitude decay below cutoff**. The left panel uses $\omega_c=\pi c/a$ and $q=\beta a/\pi$ to plot $\omega/\omega_c=\sqrt{1+q^2}$. The secant slope is [phase velocity](phase-velocity.md) divided by $c$; the tangent slope is [group velocity](group-velocity.md) divided by $c$. The right panel is the single decaying branch at $f=0.8f_c$, not an experimental transmission curve or a curve for dissipated [power](power.md).

**Table of contents**

- [Waveguide phase and group velocities](waveguide-phase-and-group-velocities.md)

## ↑ Ancestors (6)

1. [Rectangular electromagnetic waveguide](rectangular-electromagnetic-waveguide.md)
2. [Electromagnetic wave](electromagnetic-wave-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Electromagnetic waveguide](electromagnetic-waveguide.md)
- [Evanescent transverse electric mode in a rectangular waveguide](evanescent-transverse-electric-mode-in-a-rectangular-waveguide.md)
- [Klein-Gordon packet velocities](klein-gordon-packet-velocities.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3/37c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/17a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-1/section-a/a3/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2/section-b/b6/d/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1/section-b/b9/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2/section-a/a1/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-2/section-a/a3/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-1/section-a/a5/solution.md)
- [Slotted-line waveguide measurement](slotted-line-waveguide-measurement.md)
- [Transverse electromagnetic mode](transverse-electromagnetic-mode.md)
- [Waveguide cutoff frequency](waveguide-cutoff-frequency.md)
