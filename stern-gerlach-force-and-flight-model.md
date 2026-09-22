# Stern-Gerlach force and flight model

↑ **Parent:** [Stern-Gerlach experiment](stern-gerlach-experiment.md)

Let the [atomic beam](atomic-beam.md) travel along $x$, with [velocity](velocity.md) $v>0$, and let $z$ measure displacement along the dominant [magnetic field](magnetic-field-split.md) [gradient](gradient.md). For a fixed effective [magnetic moment](magnetic-dipole-moment.md) component $\mu_z$, the [magnetic dipole potential energy](magnetic-dipole-potential-energy.md) is $U\simeq-\mu_zB_z$. Taking its negative [partial derivative](partial-derivative.md) gives

$$
F_z=-\frac{\partial U}{\partial z}\simeq\mu_z\frac{\partial B_z}{\partial z}=\mu_zG.
$$

A spatially uniform [magnetic field](magnetic-field-split.md) can produce [torque](torque.md) and [Larmor precession](larmor-precession.md), but cannot produce this translational separation. In a [quantum state](quantum-state.md) following a local internal [energy eigenvalue](energy-eigenvalue-split.md) $E_n(B)$, the more general expression is $F_z=-\partial_zE_n$, with effective [magnetic moment](magnetic-dipole-moment.md) $-\partial E_n/\partial B$. Treating that moment as constant is an approximation with a physical regime, not an extra measured fact. Assume the local [magnetic field](magnetic-field-split.md) direction stays nearly fixed across the sampled beam, and that internal states follow it without transitions, as in the [adiabatic theorem](adiabatic-theorem.md). The scalar [gradient](gradient.md) model describes the beam's neighborhood; it omits the full [magnetic field](magnetic-field-split.md)'s transverse components and fringe regions.

Assume a constant $G$ over magnet length $\ell$, followed by a field-free drift $D$. Neglect transverse motion at entry and changes in longitudinal [velocity](velocity.md). [Newton's second law](newton-s-second-law.md) gives transverse [acceleration](acceleration.md) $a_z=\mu_zG/M$ for whole-atom [mass](mass.md) $M$. The magnet transit time is $t_m=\ell/v$, and the drift time is $t_d=D/v$. The magnet supplies both a displacement and an exit transverse [velocity](velocity.md):

$$
z_m-z_0=\frac{a_zt_m^2}{2},\qquad
v_{z,m}=a_zt_m,\qquad
z_s-z_0=\frac{\mu_zG}{Mv^2}\left(\frac{\ell^2}{2}+\ell D\right).
$$

The $\ell D$ contribution is motion with the acquired transverse [velocity](velocity.md), not continued [acceleration](acceleration.md) outside the magnet. For the plate-at-exit geometry, set $D=0$. For a nonzero entrance transverse [velocity](velocity.md) $w$, add $w(\ell+D)/v$. These terms show why initial [collimation](collimation.md) and flight geometry matter when inferring a [magnetic moment](magnetic-dipole-moment.md) from a deposit.

Choose hypothetical parameters $M=1.79\times10^{-25}\,\mathrm{kg}$, $G=300\,\mathrm{T\,m^{-1}}$, $\ell=0.035\,\mathrm m$, $D=0.100\,\mathrm m$, and $v=500\,\mathrm{m\,s^{-1}}$. Approximate the two effective [magnetic moments](magnetic-dipole-moment.md) by $\mu_z=\pm\mu_B$, where the [Bohr magneton](bohr-magneton.md) is $\mu_B\simeq9.274\times10^{-24}\,\mathrm{J\,T^{-1}}$. Then $|a_z|\simeq1.55\times10^4\,\mathrm{m\,s^{-2}}$, $t_m=70\,\mu\mathrm s$ and $t_d=200\,\mu\mathrm s$. The positive displacement is about $0.0381\,\mathrm{mm}$ inside the magnet plus $0.2176\,\mathrm{mm}$ during drift: $d=0.2557\,\mathrm{mm}$, with full separation $2d=0.5114\,\mathrm{mm}$. These chosen values illustrate the model and are not reconstructed 1922 measurements.

The exit transverse [velocity](velocity.md) is only about $1.09\,\mathrm{m\,s^{-1}}$, small compared with the chosen forward [velocity](velocity.md); this checks the small-deflection assumption. Halving $G$ halves $d$, doubling $v$ divides $d$ by four, and setting $D=0$ removes most of this example's separation. A real pole has fringe [magnetic fields](magnetic-field-split.md) and a position-dependent [gradient](gradient.md); these require a more complete trajectory calculation.

## ↑ Ancestors (7)

1. [Stern-Gerlach experiment](stern-gerlach-experiment.md)
2. [Spin](spin.md)
3. [Angular momentum operator](angular-momentum-operator-split.md)
4. [Quantum mechanics](quantum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
