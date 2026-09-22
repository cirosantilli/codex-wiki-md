# Electrostatics

↑ **Parent:** [Electromagnetism](electromagnetism-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Electrostatics)

[Electrostatics](electrostatics.md) studies time-independent [electric charge](electric-charge.md) distributions and their [electric fields](electric-field.md). In [vacuum](vacuum.md), its local equations in [SI](international-system-of-units.md) units are

$$
\nabla\cdot\mathbf E=\frac{\rho}{\epsilon_0},\qquad \nabla\times\mathbf E=\mathbf0,\qquad \mathbf E=-\nabla\Phi,\qquad \nabla^2\Phi=-\frac{\rho}{\epsilon_0}.
$$

Here $\rho$ is [charge density](charge-density.md), $\epsilon_0$ is [vacuum permittivity](vacuum-permittivity.md), and $\Phi$ is [electric potential](electric-potential.md). [Gauss's law](gauss-s-law.md) supplies the [divergence](divergence.md) equation; the static form of [Faraday's law of induction](faraday-s-law-of-induction.md) supplies the zero [curl](curl.md). The [Poisson equation](poisson-equation.md) becomes [Laplace's equation](laplace-equation.md) where there is no [electric charge](electric-charge.md). Prescribed [electric charges](electric-charge.md) give [electric fields](electric-field.md) through [Coulomb's law](coulomb-s-law.md) and the [superposition principle](superposition-principle.md); mobile [electric charges](electric-charge.md) on an [electrical conductor](electrical-conductor.md) instead require solving for their distribution together with the [electric potential](electric-potential.md). [Richard Fitzpatrick, Electrostatics and magnetostatics: field equations and boundary data](https://farside.ph.utexas.edu/teaching/em/lectures/node40.html).

The useful distinction is between prescribed sources and prescribed [boundary conditions](boundary-condition.md). On a grounded [electrical conductor](electrical-conductor.md), an external connection fixes its [electric potential](electric-potential.md) relative to an [electrical reference potential](electrical-reference-potential.md) and allows [electric charge](electric-charge.md) to enter or leave. On an isolated [electrical conductor](electrical-conductor.md), total [electric charge](electric-charge.md) is fixed and its constant [electric potential](electric-potential.md) is an unknown. A neutral isolated [electrical conductor](electrical-conductor.md) can therefore have a nonzero local [surface charge density](surface-charge-density.md) through [electrostatic induction](electrostatic-induction.md). Equal [electric potentials](electric-potential.md) also do not imply equal [electric charges](electric-charge.md): [charge sharing between distant connected spheres](charge-sharing-between-distant-connected-spheres.md) gives a simple geometric example. [Feynman, Leighton and Sands, II.6: charged conductors and connected-sphere estimates](https://www.feynmanlectures.caltech.edu/II_06.html#Ch6-S6).

[Electrostatics](electrostatics.md) is useful because a spatial [boundary value problem](boundary-value-problem.md) replaces the need to follow every moving [charge carrier](charge-carrier.md) during [charge relaxation](charge-relaxation.md). It describes the settled state of a [capacitor](capacitor.md) and explains [electrostatic shielding](electrostatic-shielding.md) of sensitive equipment. Its assumptions must match the apparatus: stationary boundaries and sources, negligible time variation of the [magnetic field](magnetic-field.md), and enough time for [charge relaxation](charge-relaxation.md). A metal carrying a maintained [electric current](electric-current.md) through finite [electrical resistance](electrical-resistance.md) generally needs a nonzero internal [electric field](electric-field.md) by [Ohm's law](ohm-s-law.md); it is not a [conductor in electrostatic equilibrium](conductor-in-electrostatic-equilibrium.md). Static macroscopic [electric charge](electric-charge.md) also does not mean that every [Electron](electron.md) is motionless. [Feynman, Leighton and Sands, II.7.1: conductor potentials as boundary-value problems](https://www.feynmanlectures.caltech.edu/II_07.html#Ch7-S1).

**Table of contents**

- [Faraday's ice pail experiment](faraday-s-ice-pail-experiment.md)
- [Electrostatic interface boundary conditions](electrostatic-interface-boundary-conditions.md)
- [Debye–Hückel approximation](debye-huckel-approximation.md)
  - [Screened sinusoidal surface-charge mode](screened-sinusoidal-surface-charge-mode.md)
    - [Phase registration of screened charged sheets](phase-registration-of-screened-charged-sheets.md)
- [Bjerrum length](bjerrum-length.md)
- [Poisson-Boltzmann equation](poisson-boltzmann-equation.md)
  - [Neutral cylindrical cell model](neutral-cylindrical-cell-model.md)
    - [Infinite-dilution limit of cylindrical counterions](infinite-dilution-limit-of-cylindrical-counterions.md)
  - [Cylindrical counterion-only Poisson-Boltzmann profile](cylindrical-counterion-only-poisson-boltzmann-profile.md)
  - [Counterion condensation](counterion-condensation.md)
    - [Manning condensed fraction](manning-condensed-fraction.md)
    - [Cylindrical screening charge](cylindrical-screening-charge.md)
    - [Manning parameter](manning-parameter.md)
- [Coulomb's law](coulomb-s-law.md)
  - [Coulomb potential energy](coulomb-potential-energy.md)
- [Electrostatic equilibrium](electrostatic-equilibrium.md)
- [Conductor in electrostatic equilibrium](conductor-in-electrostatic-equilibrium.md)
  - [Cavity in a conductor](cavity-in-a-conductor.md)
  - [Electrostatic shielding](electrostatic-shielding.md)
  - [Electrostatic boundary conditions at a conductor](electrostatic-boundary-conditions-at-a-conductor.md)
    - [Surface charge density](surface-charge-density.md)
  - [Charge sharing between distant connected spheres](charge-sharing-between-distant-connected-spheres.md)
  - [Charge on connected concentric spherical shells](charge-on-connected-concentric-spherical-shells.md)
  - [Induced charge on a conducting sphere in a uniform electric field](induced-charge-on-a-conducting-sphere-in-a-uniform-electric-field.md)
- [Electrostatic energy](electrostatic-energy.md)
  - [Electrostatic energy of a three-plate capacitor](electrostatic-energy-of-a-three-plate-capacitor.md)
  - [Electrostatic energy of a uniformly charged solid sphere](electrostatic-energy-of-a-uniformly-charged-solid-sphere.md)
  - [Electrostatic energy of alternating-charge concentric shells](electrostatic-energy-of-alternating-charge-concentric-shells.md)
  - [Electrostatic energy of a uniformly charged spherical shell](electrostatic-energy-of-a-uniformly-charged-spherical-shell.md)
  - [Electrostatic potential energy of point charges](electrostatic-potential-energy-of-point-charges.md)
  - [Coaxial cylindrical capacitor](coaxial-cylindrical-capacitor.md)
    - [Coaxial capacitor with grounded inner and outer cylinders](coaxial-capacitor-with-grounded-inner-and-outer-cylinders.md)
- [Electric dipole moment](electric-dipole-moment.md)
  - [Time derivative of the electric dipole moment](time-derivative-of-the-electric-dipole-moment.md)
  - [Electric dipole](electric-dipole.md)
    - [Electric dipole-dipole interaction](electric-dipole-dipole-interaction.md)
- [Electric multipole expansion](electric-multipole-expansion.md)
  - [Electric quadrupole moment](electric-quadrupole-moment.md)
  - [Electric quadrupole](electric-quadrupole.md)
  - [Multipole expansion of three collinear charges](multipole-expansion-of-three-collinear-charges.md)
    - [Dipole and quadrupole scaling limits of three collinear charges](dipole-and-quadrupole-scaling-limits-of-three-collinear-charges.md)
    - [Transverse force from a collinear electric quadrupole](transverse-force-from-a-collinear-electric-quadrupole.md)

## ↑ Ancestors (4)

1. [Electromagnetism](electromagnetism-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Active site](active-site.md)
- [Bounded two-dimensional capacitor field model](bounded-two-dimensional-capacitor-field-model.md)
- [Electric dipole](electric-dipole.md)
- [Electric potential](electric-potential.md)
- [Electric potential difference](electric-potential-difference.md)
- [Electrostatic boundary conditions at a conductor](electrostatic-boundary-conditions-at-a-conductor.md)
- [Electrostatics](electrostatics.md)
- [Faraday's ice pail experiment](faraday-s-ice-pail-experiment.md)
- [Gauss's law](gauss-s-law.md)
- [Ionic bonding](ionic-bonding.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-71/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1/16d/a/solution.md)
- [Rayleigh scattering by a small sphere](rayleigh-scattering-by-a-small-sphere.md)
