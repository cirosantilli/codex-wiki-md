# Evanescent probability current

↑ **Parent:** [Quantum tunnelling](quantum-tunnelling.md)

A nonzero [probability density](probability-density.md) inside a barrier does not by itself imply transport. In one dimension, the [probability current](probability-current.md) of a [wavefunction](wave-function.md) is $J=(\hbar/m)\operatorname{Im}(\psi^*\psi')$. A single [evanescent wave](evanescent-wave.md) $Ce^{-\kappa x}$ has $\psi^*\psi'=-\kappa|C|^2e^{-2\kappa x}$, a real quantity, hence $J=0$. This is what happens on the inaccessible side of a [potential barrier](potential-barrier.md) extending to infinity with $E<V_0$.[p. 5, equations (3.4)-(3.6): probability continuity equation and probability current](quantum-physics-i-8-04-spring-2016/lecture-6.md)

For the finite-barrier [wavefunction](wave-function.md) $Ae^{\kappa x}+Be^{-\kappa x}$, the cross terms instead give

$$
J=\frac{2\hbar\kappa}{m}\operatorname{Im}(B^*A).
$$

The relative [quantum phase](quantum-phase.md) of the two [probability amplitudes](probability-amplitude.md) permits a nonzero, spatially constant [probability current](probability-current.md), even though neither [exponential function](exponential-function.md) separately carries it. The [probability continuity equation](probability-continuity-equation.md) gives $\partial_xJ=0$ for this [stationary state](stationary-state.md). Matching the [wavefunction](wave-function.md) and its [derivative](derivative.md) also makes $J$ continuous at both faces, so

$$
J_{\mathrm{inc}}=\frac{\hbar k}{m},\qquad
J_{\mathrm{ref}}=-\frac{\hbar k}{m}|r|^2,\qquad
J_{\mathrm{tr}}=\frac{\hbar k}{m}|t|^2,\qquad
R+T=1.
$$

Here $R=|r|^2$ is the [quantum reflection probability](quantum-reflection-probability.md), and $T=J_{\mathrm{tr}}/J_{\mathrm{inc}}$ is the [transmission probability](transmission-probability.md). The net exterior [probability current](probability-current.md) equals the interior [probability current](probability-current.md); it is not lost as the [wavefunction](wave-function.md) decreases. A physical incident [wave packet](wave-packet.md) supplies finite total probability, while the [stationary state](stationary-state.md) describes the [energy](energy.md) component used to compute its transmitted flux.

## ↑ Ancestors (6)

1. [Quantum tunnelling](quantum-tunnelling.md)
2. [Potential barrier](potential-barrier.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
