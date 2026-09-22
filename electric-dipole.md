# Electric dipole

↑ **Parent:** [Electric dipole moment](electric-dipole-moment.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Electric_dipole)

A finite [electric dipole](electric-dipole.md) consists of equal and opposite [electric charges](electric-charge-split.md) separated by a nonzero [displacement](displacement.md). It has [charge neutrality](charge-neutrality.md) but a nonzero [electric dipole moment](electric-dipole-moment.md) $\mathbf p=q\mathbf d$. An ideal point [electric dipole](electric-dipole.md) is the mathematical limit $d=|\mathbf d|\to0$ with $\mathbf p$ fixed, so $q$ must increase as $1/d$. Shrinking the separation while holding $q$ fixed instead makes the [electric dipole moment](electric-dipole-moment.md) vanish. The ideal [electric dipole](electric-dipole.md) describes an exterior [electric field](electric-field-split.md); it does not reproduce the two near-charge singularities or the internal structure of a [molecule](molecule-split.md). [Richard Fitzpatrick, Electric Dipoles: the fixed-moment point limit](https://farside.ph.utexas.edu/teaching/jk1/lectures/node20.html).

Place the pair's midpoint at the origin and write $k_e=1/(4\pi\epsilon_0)$, where $\epsilon_0$ is [vacuum permittivity](vacuum-permittivity.md). By [superposition principle](superposition-principle.md) and [Coulomb's law](coulomb-s-law.md), its exact [electric potential](electric-potential.md) away from the two [point charges](point-charge.md) is

$$
\Phi_{\rm pair}(\mathbf r)=k_eq\left(\frac1{|\mathbf r-\mathbf d/2|}-\frac1{|\mathbf r+\mathbf d/2|}\right).
$$

For $r=|\mathbf r|\gg d$, retain the first nonzero term of a [Taylor series](taylor-series.md). The [electric potential](electric-potential.md) and its negative [gradient](gradient.md) become

$$
\Phi_{\rm dip}(\mathbf r)=k_e\frac{\mathbf p\cdot\widehat{\mathbf r}}{r^2},
\qquad
\mathbf E_{\rm dip}(\mathbf r)=\frac{k_e}{r^3}\left[3(\mathbf p\cdot\widehat{\mathbf r})\widehat{\mathbf r}-\mathbf p\right],\qquad r>0.
$$

Here $\widehat{\mathbf r}=\mathbf r/r$ and the products in parentheses are [dot products](dot-product.md). These are exact exterior formulas for the ideal [electric dipole](electric-dipole.md) and distant approximations for a finite pair. The [electric field](electric-field-split.md) on the outer axis points along $\mathbf p$ with magnitude $2k_ep/r^3$; on the perpendicular bisector it points opposite $\mathbf p$ with magnitude $k_ep/r^3$. This directional structure is what a scalar total [electric charge](electric-charge-split.md) misses. [Feynman, Leighton and Sands, II.6.2: exact pair potential and dipole expansion](https://www.feynmanlectures.caltech.edu/II_06.html#Ch6-S2).

In a prescribed uniform external [electric field](electric-field-split.md) $\mathbf E_{\rm ext}$, a rigid pair has opposite [forces](force-split.md) $\mathbf F_\pm=\pm q\mathbf E_{\rm ext}$. Its net [force](force-split.md) is zero, but summing their moments about the midpoint gives the [torque](torque.md)

$$
\boldsymbol\tau=\frac{\mathbf d}{2}\times q\mathbf E_{\rm ext}+\left(-\frac{\mathbf d}{2}\right)\times\left(-q\mathbf E_{\rm ext}\right)=\mathbf p\times\mathbf E_{\rm ext}.
$$

The [cross product](cross-product.md) makes the [torque](torque.md) perpendicular to both the [electric dipole moment](electric-dipole-moment.md) and the external [electric field](electric-field-split.md). If $\theta$ is the angle from $\mathbf E_{\rm ext}$ to $\mathbf p$ in their plane, the signed turning [torque](torque.md) is $\tau_\theta=-pE_{\rm ext}\sin\theta$. It tends to reduce a small positive $\theta$. [Ling, Moebs and Sanny, University Physics 2, 5.7: forces and torque on a dipole](https://openstax.org/books/university-physics-volume-2/pages/5-7-electric-dipoles).

The external interaction [potential energy](potential-energy.md), with zero chosen at $\theta=\pi/2$, is

$$
U=-\mathbf p\cdot\mathbf E_{\rm ext}=-pE_{\rm ext}\cos\theta,\qquad \tau_\theta=-\frac{dU}{d\theta}.
$$

Parallel alignment minimizes this [potential energy](potential-energy.md); antiparallel alignment maximizes it even though the [torque](torque.md) is zero in both positions. This omits the pair's constant internal binding [potential energy](potential-energy.md) and assumes a fixed permanent [electric dipole moment](electric-dipole-moment.md). [Richard Fitzpatrick, Classical Electromagnetism, exercise 2.10: dipole torque and energy](https://farside.ph.utexas.edu/teaching/jk1/Electromagnetism.pdf).

<a id="image-neutral-charge-pair-and-orientation-energy-in-a-uniform-electric-field"></a>
![](electric-dipoles-pair-torque.png)

**[Figure 6](#image-neutral-charge-pair-and-orientation-energy-in-a-uniform-electric-field). Neutral charge pair and orientation energy in a uniform electric field**. Original analytical illustration for a rigid [electric dipole](electric-dipole.md). Equal opposite [forces](force-split.md) cancel in translation but give a clockwise [torque](torque.md) at the depicted positive angle. The [potential energy](potential-energy.md) curve is the dimensionless model $U/(pE_{\rm ext})=-\cos\theta$, not measured data.

A nonuniform external [electric field](electric-field-split.md) can exert a net [force](force-split.md) on a neutral [electric dipole](electric-dipole.md). Before taking the small-pair approximation, the exact external [force](force-split.md) is $\mathbf F=q[\mathbf E_{\rm ext}(\mathbf R+\mathbf d/2)-\mathbf E_{\rm ext}(\mathbf R-\mathbf d/2)]$, where $\mathbf R$ is the midpoint. A first-order [Taylor series](taylor-series.md) gives, for a fixed [electric dipole moment](electric-dipole-moment.md) and an external [electric field](electric-field-split.md) varying slowly across $d$,

$$
\mathbf F\simeq(\mathbf p\cdot\nabla)\mathbf E_{\rm ext}=\nabla(\mathbf p\cdot\mathbf E_{\rm ext})
$$

in [electrostatics](electrostatics-split.md). The last equality uses the vanishing [curl](curl.md) of the external [electric field](electric-field-split.md), with $\mathbf p$ held fixed while differentiating. Thus uniform external [electric fields](electric-field-split.md) turn a misaligned [electric dipole](electric-dipole.md), whereas gradients can also move its midpoint. For example, the local source-free [electric field](electric-field-split.md) $\mathbf E_{\rm ext}=Gx\widehat{\mathbf x}+(E_0-Gy)\widehat{\mathbf y}$ gives $\mathbf F=(Gp_x,-Gp_y,0)$, so reversing the [electric dipole moment](electric-dipole-moment.md) reverses the net [force](force-split.md). This stipulated local model has zero [divergence](divergence.md) and zero [curl](curl.md).

A motivating experiment is Filsinger and colleagues' study of electrostatic deflection of [polar molecules](polar-molecule.md). Benzonitrile ($\mathrm{C_7H_5N}$) in [helium](helium.md) expanded from a pulsed valve into [vacuum](vacuum.md); two 1-mm skimmers narrowed the beam before a 15-cm deflector. A grounded trough and a high-voltage rod produced a vertical [electric field](electric-field-split.md) gradient. Scanning a focused [laser](laser-split.md) vertically downstream and recording benzonitrile ions from [photoionization](photoionization.md) measured the beam's relative density. With voltage off, the profile spanned about 2 mm; applying voltage shifted and broadened it upwards. At 10 kV, many [molecules](molecule-split.md) lay outside the original profile. [Filsinger et al., Quantum state selection, alignment, and orientation of large molecules using static electric and laser fields, sections II and III A, figure 3](https://pure.mpg.de/pubman/item/item_736019_2/component/file_736018/433451%28filsinger%29.pdf).

Interpretation uses a [quantum state](quantum-state.md)'s [Stark effect](stark-effect.md) [energy](energy-split.md) $W(E)$: $\mu_{\rm eff}=-dW/dE$ gives $F_y=\mu_{\rm eff}\,\partial_yE$. States whose [energy](energy-split.md) falls with increasing [electric field](electric-field-split.md) seek stronger fields. The voltage-off profile controls the mechanical aperture. Inferring state populations needs calculated trajectories, [speed](speed.md) distributions and a rotational [temperature](temperature-split.md) model; profile displacement alone does not measure a permanent [electric dipole moment](electric-dipole-moment.md) uniquely. This is an electric [Stark effect](stark-effect.md) experiment, with [photoionization](photoionization.md) occurring after deflection. [Filsinger et al., section III A: Stark slopes, trajectory modelling and state selection](https://pure.mpg.de/pubman/item/item_736019_2/component/file_736018/433451%28filsinger%29.pdf).

For the symmetric finite pair, the first omitted [electric multipole expansion](electric-multipole-expansion.md) term after the [electric dipole](electric-dipole.md) is third order, so typical relative errors scale as $(d/r)^2$. This stronger error estimate need not hold for an arbitrary neutral [molecule](molecule-split.md) with a nonzero [electric quadrupole moment](electric-quadrupole-moment.md). A concrete check for a pair on the $z$ axis compares the exact and ideal [electric fields](electric-field-split.md) at $r>d/2$ on the positive axis and at $r>0$ on the perpendicular bisector:

$$
\frac{E_{z,\rm pair}(0,0,r)}{E_{z,\rm dip}(0,0,r)}=\left(1-\frac{d^2}{4r^2}\right)^{-2},
\qquad
\frac{E_{z,\rm pair}(r,0,0)}{E_{z,\rm dip}(r,0,0)}=\left(1+\frac{d^2}{4r^2}\right)^{-3/2}.
$$

Both perpendicular-bisector components are negative. At $r=5d$, the ratios are approximately $1.0203$ and $0.9852$: errors of $+2.03\%$ and $-1.48\%$ relative to the ideal [electric field](electric-field-split.md). The condition $r\gg d$ concerns observing the pair's own [electric field](electric-field-split.md); the separate condition for its external [force](force-split.md) approximation concerns variation of the applied [electric field](electric-field-split.md) across the pair.

<a id="image-finite-charge-pair-approaching-its-ideal-electric-dipole-field"></a>
![](electric-dipoles-finite-field.png)

**[Figure 7](#image-finite-charge-pair-approaching-its-ideal-electric-dipole-field). Finite charge pair approaching its ideal electric dipole field**. Original geometry and analytical field-ratio curves for two [point charges](point-charge.md) $\pm q$ separated by $d$. The outer axial [electric field](electric-field-split.md) points along the [electric dipole moment](electric-dipole-moment.md); the perpendicular-bisector [electric field](electric-field-split.md) points against it. The curves compare exact [Coulomb's law](coulomb-s-law.md) sums with the ideal [electric dipole](electric-dipole.md) prediction and are models, not experimental measurements.

**Table of contents**

- [Electric dipole field](electric-dipole-field.md)
- [Electric dipole-dipole interaction](electric-dipole-dipole-interaction.md)
  - [Transverse electric-dipole pair energy](transverse-electric-dipole-pair-energy.md)
  - [Dipole depolarization](dipole-depolarization.md)

## ↑ Ancestors (6)

1. [Electric dipole moment](electric-dipole-moment.md)
2. [Electrostatics](electrostatics-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (46)

- [Ammonia inversion transition](ammonia-inversion-transition.md)
- [Attosecond streaking](attosecond-streaking.md)
- [Bulk electric-dipole selection rule](bulk-electric-dipole-selection-rule.md)
- [Dielectric](dielectric.md)
- [Electric charge](electric-charge-split.md)
- [Electric dipole](electric-dipole.md)
- [Electric dipole-dipole interaction](electric-dipole-dipole-interaction.md)
- [Electric dipole moment](electric-dipole-moment.md)
- [Electric-dipole radar cross section of a small conducting sphere](electric-dipole-radar-cross-section-of-a-small-conducting-sphere.md)
- [Electric flux](electric-flux.md)
- [Electric potential](electric-potential.md)
- [Electrostatic boundary conditions at a conductor](electrostatic-boundary-conditions-at-a-conductor.md)
- [Förster resonance energy transfer](forster-resonance-energy-transfer.md)
- [FRET dipole orientation factor](fret-dipole-orientation-factor.md)
- [Hertzian dipole](hertzian-dipole.md)
- [Infrared](infrared.md)
- [Ion-dipole attraction](ion-dipole-attraction.md)
- [Lennard-Jones potential](lennard-jones-potential.md)
- [Linear molecule](linear-molecule.md)
- [London dispersion force](london-dispersion-force.md)
- [Maser oscillation threshold](maser-oscillation-threshold.md)
- [Microscopic dielectric polarization](microscopic-dielectric-polarization.md)
- [Outgoing radiation pulse](outgoing-radiation-pulse.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-2/16d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1/15d/b/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2013/paper-1/2/b/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2015/paper-1/3/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2021/section-a/a1/a/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2021/section-a/a1/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1/section-b/b6/b/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2/section-b/b6/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2/section-b/b7/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-1/section-c/c8/f/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2/section-b/b7/b/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/section-e/e15/a/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/section-e/e15/b/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/section-e/15/a/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/section-b/10/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2007/section-a/a1/c/solution.md)
- [Permittivity](permittivity-split.md)
- [Pure rotational electric-dipole selection rules](pure-rotational-electric-dipole-selection-rules.md)
- [Rayleigh optical gradient force](rayleigh-optical-gradient-force.md)
- [Rayleigh scattering](rayleigh-scattering.md)
- [Rayleigh scattering angular pattern](rayleigh-scattering-angular-pattern.md)
- [Stark effect of the hydrogen ground state](stark-effect-of-the-hydrogen-ground-state.md)
- [Three-level observable and missing spectral line](three-level-observable-and-missing-spectral-line.md)
