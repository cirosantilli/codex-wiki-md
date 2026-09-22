# Electric dipole

↑ **Parent:** [Electric dipole moment](electric-dipole-moment.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Electric_dipole)

A finite [electric dipole](electric-dipole.md) consists of equal and opposite [electric charges](electric-charge.md) separated by a nonzero [displacement](displacement.md). It has [charge neutrality](charge-neutrality.md) but a nonzero [electric dipole moment](electric-dipole-moment.md) $\mathbf p=q\mathbf d$. An ideal point [electric dipole](electric-dipole.md) is the mathematical limit $d=|\mathbf d|\to0$ with $\mathbf p$ fixed, so $q$ must increase as $1/d$. Shrinking the separation while holding $q$ fixed instead makes the [electric dipole moment](electric-dipole-moment.md) vanish. The ideal [electric dipole](electric-dipole.md) describes an exterior [electric field](electric-field.md); it does not reproduce the two near-charge singularities or the internal structure of a [molecule](molecule.md). [Richard Fitzpatrick, Electric Dipoles: the fixed-moment point limit](https://farside.ph.utexas.edu/teaching/jk1/lectures/node20.html).

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

Here $\widehat{\mathbf r}=\mathbf r/r$ and the products in parentheses are [dot products](dot-product.md). These are exact exterior formulas for the ideal [electric dipole](electric-dipole.md) and distant approximations for a finite pair. The [electric field](electric-field.md) on the outer axis points along $\mathbf p$ with magnitude $2k_ep/r^3$; on the perpendicular bisector it points opposite $\mathbf p$ with magnitude $k_ep/r^3$. This directional structure is what a scalar total [electric charge](electric-charge.md) misses. [Feynman, Leighton and Sands, II.6.2: exact pair potential and dipole expansion](https://www.feynmanlectures.caltech.edu/II_06.html#Ch6-S2).

In a prescribed uniform external [electric field](electric-field.md) $\mathbf E_{\rm ext}$, a rigid pair has opposite [forces](force.md) $\mathbf F_\pm=\pm q\mathbf E_{\rm ext}$. Its net [force](force.md) is zero, but summing their moments about the midpoint gives the [torque](torque.md)

$$
\boldsymbol\tau=\frac{\mathbf d}{2}\times q\mathbf E_{\rm ext}+\left(-\frac{\mathbf d}{2}\right)\times\left(-q\mathbf E_{\rm ext}\right)=\mathbf p\times\mathbf E_{\rm ext}.
$$

The [cross product](cross-product.md) makes the [torque](torque.md) perpendicular to both the [electric dipole moment](electric-dipole-moment.md) and the external [electric field](electric-field.md). If $\theta$ is the angle from $\mathbf E_{\rm ext}$ to $\mathbf p$ in their plane, the signed turning [torque](torque.md) is $\tau_\theta=-pE_{\rm ext}\sin\theta$. It tends to reduce a small positive $\theta$. [Ling, Moebs and Sanny, University Physics 2, 5.7: forces and torque on a dipole](https://openstax.org/books/university-physics-volume-2/pages/5-7-electric-dipoles).

The external interaction [potential energy](potential-energy.md), with zero chosen at $\theta=\pi/2$, is

$$
U=-\mathbf p\cdot\mathbf E_{\rm ext}=-pE_{\rm ext}\cos\theta,\qquad \tau_\theta=-\frac{dU}{d\theta}.
$$

Parallel alignment minimizes this [potential energy](potential-energy.md); antiparallel alignment maximizes it even though the [torque](torque.md) is zero in both positions. This omits the pair's constant internal binding [potential energy](potential-energy.md) and assumes a fixed permanent [electric dipole moment](electric-dipole-moment.md). [Richard Fitzpatrick, Classical Electromagnetism, exercise 2.10: dipole torque and energy](https://farside.ph.utexas.edu/teaching/jk1/Electromagnetism.pdf).

<a id="image-neutral-charge-pair-and-orientation-energy-in-a-uniform-electric-field"></a>
![](electric-dipoles-pair-torque.png)

**[Figure 43](#image-neutral-charge-pair-and-orientation-energy-in-a-uniform-electric-field). Neutral charge pair and orientation energy in a uniform electric field**. Original analytical illustration for a rigid [electric dipole](electric-dipole.md). Equal opposite [forces](force.md) cancel in translation but give a clockwise [torque](torque.md) at the depicted positive angle. The [potential energy](potential-energy.md) curve is the dimensionless model $U/(pE_{\rm ext})=-\cos\theta$, not measured data.

A nonuniform external [electric field](electric-field.md) can exert a net [force](force.md) on a neutral [electric dipole](electric-dipole.md). Before taking the small-pair approximation, the exact external [force](force.md) is $\mathbf F=q[\mathbf E_{\rm ext}(\mathbf R+\mathbf d/2)-\mathbf E_{\rm ext}(\mathbf R-\mathbf d/2)]$, where $\mathbf R$ is the midpoint. A first-order [Taylor series](taylor-series.md) gives, for a fixed [electric dipole moment](electric-dipole-moment.md) and an external [electric field](electric-field.md) varying slowly across $d$,

$$
\mathbf F\simeq(\mathbf p\cdot\nabla)\mathbf E_{\rm ext}=\nabla(\mathbf p\cdot\mathbf E_{\rm ext})
$$

in [electrostatics](electrostatics.md). The last equality uses the vanishing [curl](curl.md) of the external [electric field](electric-field.md), with $\mathbf p$ held fixed while differentiating. Thus uniform external [electric fields](electric-field.md) turn a misaligned [electric dipole](electric-dipole.md), whereas gradients can also move its midpoint. For example, the local source-free [electric field](electric-field.md) $\mathbf E_{\rm ext}=Gx\widehat{\mathbf x}+(E_0-Gy)\widehat{\mathbf y}$ gives $\mathbf F=(Gp_x,-Gp_y,0)$, so reversing the [electric dipole moment](electric-dipole-moment.md) reverses the net [force](force.md). This stipulated local model has zero [divergence](divergence.md) and zero [curl](curl.md).

A motivating experiment is Filsinger and colleagues' study of electrostatic deflection of [polar molecules](polar-molecule.md). Benzonitrile ($\mathrm{C_7H_5N}$) in [helium](helium.md) expanded from a pulsed valve into [vacuum](vacuum.md); two 1-mm skimmers narrowed the beam before a 15-cm deflector. A grounded trough and a high-voltage rod produced a vertical [electric field](electric-field.md) gradient. Scanning a focused [laser](laser.md) vertically downstream and recording benzonitrile ions from [photoionization](photoionization.md) measured the beam's relative density. With voltage off, the profile spanned about 2 mm; applying voltage shifted and broadened it upwards. At 10 kV, many [molecules](molecule.md) lay outside the original profile. [Filsinger et al., Quantum state selection, alignment, and orientation of large molecules using static electric and laser fields, sections II and III A, figure 3](https://pure.mpg.de/pubman/item/item_736019_2/component/file_736018/433451%28filsinger%29.pdf).

Interpretation uses a [quantum state](quantum-state.md)'s [Stark effect](stark-effect.md) [energy](energy.md) $W(E)$: $\mu_{\rm eff}=-dW/dE$ gives $F_y=\mu_{\rm eff}\,\partial_yE$. States whose [energy](energy.md) falls with increasing [electric field](electric-field.md) seek stronger fields. The voltage-off profile controls the mechanical aperture. Inferring state populations needs calculated trajectories, [speed](speed.md) distributions and a rotational [temperature](temperature.md) model; profile displacement alone does not measure a permanent [electric dipole moment](electric-dipole-moment.md) uniquely. This is an electric [Stark effect](stark-effect.md) experiment, with [photoionization](photoionization.md) occurring after deflection. [Filsinger et al., section III A: Stark slopes, trajectory modelling and state selection](https://pure.mpg.de/pubman/item/item_736019_2/component/file_736018/433451%28filsinger%29.pdf).

For the symmetric finite pair, the first omitted [electric multipole expansion](electric-multipole-expansion.md) term after the [electric dipole](electric-dipole.md) is third order, so typical relative errors scale as $(d/r)^2$. This stronger error estimate need not hold for an arbitrary neutral [molecule](molecule.md) with a nonzero [electric quadrupole moment](electric-quadrupole-moment.md). A concrete check for a pair on the $z$ axis compares the exact and ideal [electric fields](electric-field.md) at $r>d/2$ on the positive axis and at $r>0$ on the perpendicular bisector:

$$
\frac{E_{z,\rm pair}(0,0,r)}{E_{z,\rm dip}(0,0,r)}=\left(1-\frac{d^2}{4r^2}\right)^{-2},
\qquad
\frac{E_{z,\rm pair}(r,0,0)}{E_{z,\rm dip}(r,0,0)}=\left(1+\frac{d^2}{4r^2}\right)^{-3/2}.
$$

Both perpendicular-bisector components are negative. At $r=5d$, the ratios are approximately $1.0203$ and $0.9852$: errors of $+2.03\%$ and $-1.48\%$ relative to the ideal [electric field](electric-field.md). The condition $r\gg d$ concerns observing the pair's own [electric field](electric-field.md); the separate condition for its external [force](force.md) approximation concerns variation of the applied [electric field](electric-field.md) across the pair.

<a id="image-finite-charge-pair-approaching-its-ideal-electric-dipole-field"></a>
![](electric-dipoles-finite-field.png)

**[Figure 44](#image-finite-charge-pair-approaching-its-ideal-electric-dipole-field). Finite charge pair approaching its ideal electric dipole field**. Original geometry and analytical field-ratio curves for two [point charges](point-charge.md) $\pm q$ separated by $d$. The outer axial [electric field](electric-field.md) points along the [electric dipole moment](electric-dipole-moment.md); the perpendicular-bisector [electric field](electric-field.md) points against it. The curves compare exact [Coulomb's law](coulomb-s-law.md) sums with the ideal [electric dipole](electric-dipole.md) prediction and are models, not experimental measurements.

**Table of contents**

- [Electric dipole-dipole interaction](electric-dipole-dipole-interaction.md)

## ↑ Ancestors (6)

1. [Electric dipole moment](electric-dipole-moment.md)
2. [Electrostatics](electrostatics.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Electric charge](electric-charge.md)
- [Electric dipole](electric-dipole.md)
- [Electric dipole-dipole interaction](electric-dipole-dipole-interaction.md)
- [Electric dipole moment](electric-dipole-moment.md)
- [Electric flux](electric-flux.md)
- [Electric potential](electric-potential.md)
- [Electrostatic boundary conditions at a conductor](electrostatic-boundary-conditions-at-a-conductor.md)
- [Förster resonance energy transfer](forster-resonance-energy-transfer.md)
- [FRET dipole orientation factor](fret-dipole-orientation-factor.md)
- [Infrared](infrared.md)
- [Ion-dipole attraction](ion-dipole-attraction.md)
- [Linear molecule](linear-molecule.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-2/16d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1/15d/b/solution.md)
- [Permittivity](permittivity.md)
- [Pure rotational electric-dipole selection rules](pure-rotational-electric-dipole-selection-rules.md)
- [Rayleigh scattering](rayleigh-scattering.md)
- [Rayleigh scattering angular pattern](rayleigh-scattering-angular-pattern.md)
- [Stark effect of the hydrogen ground state](stark-effect-of-the-hydrogen-ground-state.md)
