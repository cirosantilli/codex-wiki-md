# Permittivity

↑ **Parent:** [Electromagnetism](electromagnetism-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Permittivity)

[Permittivity](permittivity.md) describes how an [electric field](electric-field.md) and a material's [electric polarization](polarization-density.md) combine into the [electric displacement field](electric-displacement-field.md). In a static, local response with [linearity](linearity.md) and [isotropy](isotropy.md), and no [electric polarization](polarization-density.md) at zero [electric field](electric-field.md), the [constitutive equation](constitutive-equation.md) is

$$
\mathbf D=\epsilon\mathbf E,\qquad \epsilon=\epsilon_0\epsilon_r.
$$

Here $\epsilon_0$ is [vacuum permittivity](vacuum-permittivity.md), while $\epsilon_r$ is the [relative permittivity](relative-permittivity.md), a [dimensionless quantity](dimensionless-quantity.md). The [SI](international-system-of-units.md) unit of [permittivity](permittivity.md) is [farad](farad.md) per metre, $\mathrm{F/m}$: multiplying it by an [electric field](electric-field.md) in $\mathrm{V/m}$ gives an [electric displacement field](electric-displacement-field.md) in $\mathrm{C/m^2}$. A larger positive [permittivity](permittivity.md) lets the same [parallel-plate capacitor](parallel-plate-capacitor.md) hold more plate [electric charge](electric-charge.md) at the same [electric potential difference](electric-potential-difference.md).

The material contribution is [electric polarization](polarization-density.md) $\mathbf P$, the [electric dipole moment](electric-dipole-moment.md) per unit [volume](volume.md). The [electric displacement field](electric-displacement-field.md) and [electric susceptibility](electric-susceptibility.md) $\chi_e$ satisfy

$$
\mathbf D=\epsilon_0\mathbf E+\mathbf P,\qquad
\mathbf P=\epsilon_0\chi_e\mathbf E,\qquad
\epsilon_r=1+\chi_e.
$$

Substitution gives the first [constitutive equation](constitutive-equation.md). The [electric field](electric-field.md) here is the averaged, total field inside the material, not just the field of the external plate [electric charges](electric-charge.md). The [continuum approximation](continuum-approximation.md) averages over many [chemical atoms](atom-physics.md) or [molecules](molecule.md); locality means that the [electric polarization](polarization-density.md) at a position depends on the [electric field](electric-field.md) there. Static equilibrium, fixed material conditions and sufficiently small [electric fields](electric-field.md) are needed for this scalar proportionality. [Polarization](classical-electromagnetism-an-intermediate-level-course-by-richard-fitzpatrick/polarization.md).

For an ideal [parallel-plate capacitor](parallel-plate-capacitor.md) completely filled by a uniform [dielectric](dielectric.md), hold the free plate [electric charge](electric-charge.md) magnitude $Q$ fixed and neglect the [fringing field of a capacitor](fringing-field-of-a-capacitor.md). Writing $A$ for the plate [area](surface-area.md), [Gauss's law](gauss-s-law.md) gives $D=Q/A$. Thus

$$
E=\frac{Q}{\epsilon_0\epsilon_r A},\qquad
P=\frac{Q}{A}\left(1-\frac1{\epsilon_r}\right).
$$

The [electric dipoles](electric-dipole.md) point along the [electric field](electric-field.md). Their surface [electric charges](electric-charge.md), described by [polarization density](polarization-density.md), oppose the field from the free plate [electric charges](electric-charge.md). For a hypothetical [dielectric](dielectric.md) with $\epsilon_r=4$, the internal [electric field](electric-field.md) is one quarter of its [vacuum](vacuum.md) value, while $P=3D/4$. At fixed [electric potential difference](electric-potential-difference.md) instead, the internal [electric field](electric-field.md) stays approximately $V/d$ and the plate [electric charge](electric-charge.md) grows fourfold. These are different experimental constraints. [Feynman, Leighton and Sands, II.10–3, equations (10.5)–(10.11): polarization surface charge, field reduction and capacitance](https://www.feynmanlectures.caltech.edu/II_10.html#Ch10-S3).

<a id="image-electric-polarization-and-electric-field-reduction-at-fixed-plate-electric-charge"></a>
![](dielectric-polarization-fixed-charge-fields.png)

**[Figure 14](#image-electric-polarization-and-electric-field-reduction-at-fixed-plate-electric-charge). Electric polarization and electric field reduction at fixed plate electric charge**. An original schematic and normalized model comparison for a uniform [dielectric](dielectric.md) with [relative permittivity](relative-permittivity.md) four. The arrows for [electric dipole moments](electric-dipole-moment.md) run from negative to positive [electric charge](electric-charge.md); the two field contributions oppose each other. The bar values compare [electric displacement field](electric-displacement-field.md) $D$, $\epsilon_0E$, and [electric polarization](polarization-density.md) $P$, which all have units $\mathrm{C/m^2}$. The schematic is not to microscopic scale.

[Permittivity](permittivity.md) is a useful material summary, not a universal constant of the material under every condition. [Temperature](temperature.md), [frequency](frequency.md) and [electric field](electric-field.md) strength can change the response. In a [linear anisotropic dielectric](linear-anisotropic-dielectric.md), [permittivity](permittivity.md) is a [tensor](tensor.md), $D_i=\sum_j\epsilon_{ij}E_j$, so the [electric displacement field](electric-displacement-field.md) need not be parallel to the [electric field](electric-field.md). At nonzero [frequency](frequency.md), delayed [electric polarization](polarization-density.md) requires [complex permittivity](complex-permittivity.md) and may produce [dielectric loss](dielectric-loss.md). [Feynman, Leighton and Sands, II.32–2, equations (32.5)–(32.8) and following paragraph: frequency dependence and phase lag](https://www.feynmanlectures.caltech.edu/II_32.html#Ch32-S2).

**Table of contents**

- [Dielectric](dielectric.md)
  - [Electric susceptibility](electric-susceptibility.md)
- [Complex permittivity](complex-permittivity.md)
  - [Dielectric loss](dielectric-loss.md)
  - [Dielectric relaxation](dielectric-relaxation.md)
- [Dielectric capacitance measurement](dielectric-capacitance-measurement.md)
  - [Capacitance measurement calibration](capacitance-measurement-calibration.md)
- [Vacuum permittivity](vacuum-permittivity.md)

## ↑ Ancestors (4)

1. [Electromagnetism](electromagnetism-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (23)

- [Bounded two-dimensional capacitor field model](bounded-two-dimensional-capacitor-field-model.md)
- [Capacitance](capacitance.md)
- [Capacitance measurement calibration](capacitance-measurement-calibration.md)
- [Capacitance of an isolated conducting sphere](capacitance-of-an-isolated-conducting-sphere.md)
- [Capacitor](capacitor.md)
- [Capacitor energy](capacitor-energy.md)
- [Dielectric capacitance measurement](dielectric-capacitance-measurement.md)
- [Diffusion-capacitance analogy](diffusion-capacitance-analogy.md)
- [Electric susceptibility](electric-susceptibility.md)
- [Electrostatic boundary conditions at a conductor](electrostatic-boundary-conditions-at-a-conductor.md)
- [Electrostatic interface boundary conditions](electrostatic-interface-boundary-conditions.md)
- [Fringing field of a capacitor](fringing-field-of-a-capacitor.md)
- [Guard electrode of a capacitor](guard-electrode-of-a-capacitor.md)
- [Linear anisotropic dielectric](linear-anisotropic-dielectric.md)
- [Parallel-plate capacitor](parallel-plate-capacitor.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-78/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-71/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/3/e/solution.md)
- [Permittivity](permittivity.md)
- [Rayleigh scattering by a small sphere](rayleigh-scattering-by-a-small-sphere.md)
- [Relative permittivity](relative-permittivity.md)
- [Uniaxial optical medium](uniaxial-optical-medium.md)
- [Vacuum permittivity](vacuum-permittivity.md)
