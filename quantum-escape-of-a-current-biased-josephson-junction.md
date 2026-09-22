# Quantum escape of a current-biased Josephson junction

↑ **Parent:** [Current-biased Josephson phase dynamics](current-biased-josephson-phase-dynamics.md)

[Quantum escape of a current-biased Josephson junction](quantum-escape-of-a-current-biased-josephson-junction.md) is decay of a trapped collective [quantum phase](quantum-phase.md) state through a barrier in the [tilted Josephson washboard potential](tilted-josephson-washboard-potential.md). This barrier lies in the [potential energy](potential-energy.md) of an [electrical circuit](electrical-circuit-split.md) coordinate. Transfer of [Cooper pairs](cooper-pair.md) across the physical insulating layer already supplies the [Josephson coupling energy](josephson-coupling-energy.md); it does not by itself demonstrate this further collective escape. [Single-electron superconducting tunneling](single-electron-superconducting-tunneling.md) is a third, distinct process.

At higher [temperature](temperature-split.md) $T$, [thermal activation](thermal-activation.md) instead lifts the coordinate over the barrier. In the rare-escape regime its characteristic form is the [Kramers escape rate](kramers-escape-rate.md)

$$
\Gamma_{\rm th}\simeq a_{\rm th}\frac{\omega_p}{2\pi}\exp\left(-\frac{\Delta U}{k_BT}\right),
$$

where $k_B$ is the [Boltzmann constant](boltzmann-constant.md) and the prefactor depends on [damping](damping.md) and thermal equilibration. Cooling suppresses this route. For a quasistationary [energy level](energy-level.md) at [energy](energy-split.md) $E$, the leading conservative [WKB approximation](wkb-approximation.md) instead has

$$
\Gamma_E\ \propto\ \exp\left[-\frac{2}{\hbar}\int_{\phi_1}^{\phi_2}\sqrt{2M_\phi\left(U(\phi)-E\right)}\,d\phi\right],
$$

with the two turning points bracketing the forbidden barrier. This is an exponential estimate requiring a large action compared with $\hbar$, slow escape compared with intrawell motion, and weak environmental corrections. It is not a complete rate prediction near the barrier top or with substantial [damping](damping.md).

The familiar cubic-barrier exponent can be checked independently. Choose $V(x)=M_\phi\omega_p^2x^2(1-x/a)/2$, with $a>0$. Its top is at $2a/3$ and $\Delta U=2M_\phi\omega_p^2a^2/27$. At the well-bottom reference [energy](energy-split.md) $E=0$,

$$
B=\frac{2M_\phi\omega_p}{\hbar}\int_0^a x\sqrt{1-x/a}\,dx
=\frac{8M_\phi\omega_pa^2}{15\hbar}
=\frac{36\Delta U}{5\hbar\omega_p}.
$$

Substitution $u=x/a$ reduces the dimensionless [integral](integral-split.md) to $\int_0^1u\sqrt{1-u}\,du=4/15$. This leading semiclassical action uses a cubic potential and a well-bottom reference; actual ground-state escape also needs the zero-point correction, prefactor and environment. In the chosen washboard example it gives $B\simeq74.0$ after matching the exact barrier and curvature. This matching is an illustrative approximation, not an exact action integral for the cosine potential.

Escape need not yield a sustained voltage: the coordinate can become trapped again. The running-state readout assumes sufficient [underdamping](underdamping.md) and bias to avoid such retrapping. The parallel model has [quality factor](q-factor.md) $Q=\omega_pRC$; large $Q$ makes energy loss per oscillation small. Low-temperature rate saturation alone cannot distinguish [quantum tunnelling](quantum-tunnelling.md) from unwanted heating or external noise.

## ↑ Ancestors (7)

1. [Current-biased Josephson phase dynamics](current-biased-josephson-phase-dynamics.md)
2. [Josephson junction](josephson-junction.md)
3. [Superconductivity](superconductivity-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Current-biased Josephson phase dynamics](current-biased-josephson-phase-dynamics.md)
- [Quantum escape of a current-biased Josephson junction](quantum-escape-of-a-current-biased-josephson-junction.md)
