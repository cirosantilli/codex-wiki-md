# Wannier-Mott exciton

↑ **Parent:** [Exciton](exciton.md)

A [Wannier-Mott exciton](wannier-mott-exciton.md) has an internal [wave function](wave-function.md) extending over many [unit cells](unit-cell.md). Its simplest model assumes a three-dimensional bulk crystal, approximately parabolic [valence band](valence-band.md) and [conduction band](conduction-band.md), positive isotropic scalar [effective masses](band-effective-mass.md) $m_e^*,m_h^*$, a constant scalar [relative permittivity](relative-permittivity.md) $\epsilon_r$, and a dilute pair population. Replace microscopic crystal forces by those [effective masses](band-effective-mass.md) and [dielectric screening](dielectric-screening.md), and neglect exchange corrections and coupling to [phonons](phonon.md). These assumptions must hold on the spatial and [energy](energy.md) scales of the particular [exciton](exciton.md).

With relative coordinate $\mathbf r=\mathbf r_e-\mathbf r_h$, the internal [Hamiltonian operator](hamiltonian-quantum-mechanics.md) is the three-dimensional [hydrogen atom](hydrogen-atom.md) problem with a [reduced mass](reduced-mass.md) and a screened [Coulomb potential](coulomb-potential-energy.md):

$$
H_{\rm rel}=-\frac{\hbar^2}{2\mu}\nabla_{\mathbf r}^2-\frac{e^2}{4\pi\epsilon_0\epsilon_r r},\qquad
\mu=\frac{m_e^*m_h^*}{m_e^*+m_h^*},\qquad M=m_e^*+m_h^*.
$$

Here $e$ is the [elementary charge](elementary-charge.md), $\epsilon_0$ the [vacuum permittivity](vacuum-permittivity.md), and $\hbar$ the reduced [Planck constant](planck-constant.md). The internal [energy eigenvalues](energy-eigenvalue.md), radius scale, and [exciton binding energies](exciton-binding-energy.md) are

$$
a_B^*=\frac{4\pi\epsilon_0\epsilon_r\hbar^2}{\mu e^2},\qquad
R^*=\frac{\mu e^4}{2(4\pi\epsilon_0\epsilon_r)^2\hbar^2},\qquad
E_{{\rm rel},n}=-\frac{R^*}{n^2},\qquad E_{B,n}=\frac{R^*}{n^2}.
$$

The [principal quantum number](principal-quantum-number.md) is $n=1,2,\ldots$. This reduction and these scales are derived in [Excitons in Semiconductor Quantum Dots by Matjaž Humar](excitons-in-semiconductor-quantum-dots-by-matjaz-humar.md) (§3, printed pp. 5–6, equations (13)–(26)).

To check the scales by [dimensional analysis](dimensional-analysis.md), write $C=e^2/(4\pi\epsilon_0\epsilon_r)$, which has units of [energy](energy.md) times [length](length.md). Then $a_B^*=\hbar^2/(\mu C)$ is a [length](length.md) and $R^*=\mu C^2/(2\hbar^2)$ is an [energy](energy.md). Rescaling $r=a_B^*\rho$ makes $H_{\rm rel}/R^*=-\nabla_\rho^2-2/\rho$, the dimensionless [hydrogen atom](hydrogen-atom.md) operator. The [Bohr radius](bohr-radius.md) $a_B^*$ is a [wave function](wave-function.md) scale, not the radius of a classical orbit; for this model's lowest internal [bound state](bound-state.md), the mean separation is $3a_B^*/2$.

For the diagrams' hypothetical inputs $m_e^*=0.10m_0$, $m_h^*=0.40m_0$, $\epsilon_r=10$ and $E_g=1.500\,\mathrm{eV}$, where $m_0$ is the free [Electron](electron.md) mass, independent substitution gives $\mu=0.080m_0$, $a_B^*\simeq6.615\,\mathrm{nm}$ and $R^*\simeq10.885\,\mathrm{meV}$. Here [electronvolts](electronvolt.md) express [energy](energy.md). The [exciton binding energies](exciton-binding-energy.md) for $n=1,2,3$ are approximately $10.885$, $2.721$ and $1.209\,\mathrm{meV}$. These are model calculations, not measured material parameters. The large-radius approximation additionally requires $a_B^*$ to be much larger than the crystal's [unit cell](unit-cell.md) length scale. In a thin layer, with anisotropic [effective masses](band-effective-mass.md), or with spatially varying [dielectric screening](dielectric-screening.md), this three-dimensional formula is not generally valid.

**Table of contents**

- [Relative permittivity](relative-permittivity.md)
  - [Dielectric screening](dielectric-screening.md)

## ↑ Ancestors (6)

1. [Exciton](exciton.md)
2. [Quasiparticle](quasiparticle.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Dielectric screening](dielectric-screening.md)
- [Exciton](exciton.md)
- [Exciton optical transition](exciton-optical-transition.md)
- [Frenkel exciton](frenkel-exciton.md)
- [Relative permittivity](relative-permittivity.md)
- [Wannier-Mott exciton](wannier-mott-exciton.md)
