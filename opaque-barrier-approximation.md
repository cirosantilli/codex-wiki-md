# Opaque barrier approximation

↑ **Parent:** [Rectangular barrier transmission probability](rectangular-barrier-transmission-probability.md)

For fixed $0<E<V_0$ and $\kappa a\gg1$, the exact [rectangular barrier transmission probability](rectangular-barrier-transmission-probability.md) gives

$$
T\sim\frac{16E(V_0-E)}{V_0^2}\exp\!\left[-\frac{2a\sqrt{2m(V_0-E)}}{\hbar}\right].
$$

This is the leading term of an [asymptotic expansion](asymptotic-expansion.md): the [wavefunction](wave-function.md) amplitude scale is $e^{-\kappa a}$, and the [transmission probability](transmission-probability.md) scale is $e^{-2\kappa a}$, with an interface prefactor. Increasing width by $\Delta a$ multiplies this approximation by $e^{-2\kappa\Delta a}$. At fixed incident [energy](energy.md), increasing barrier height increases the [tunnelling decay constant](tunnelling-decay-constant.md) as $\sqrt{V_0-E}$; heavier [nonrelativistic particles](nonrelativistic-particle.md) also have stronger suppression. For the numerical example in [rectangular barrier transmission probability](rectangular-barrier-transmission-probability.md), the approximation gives $0.01397$, compared with the exact $0.01388$.

The regime condition matters. Near $E=V_0$ at fixed width, $\kappa a$ tends to zero and the [opaque barrier approximation](opaque-barrier-approximation.md) fails; use the exact threshold value. For $\kappa a\ll1$, expansion of the [hyperbolic sine](hyperbolic-sine.md) gives

$$
T\simeq\left[1+\frac{mV_0^2a^2}{2\hbar^2E}\right]^{-1}.
$$

This tends to one as $a\to0$ at fixed $E,V_0$, but the condition $\kappa a\ll1$ alone does not imply nearly perfect transmission if the remaining factor is large. At $E>V_0$, use the oscillatory formula and its [scattering resonances](scattering-resonance.md), rather than an [exponential decay](exponential-decay.md) law.

## ↑ Ancestors (8)

1. [Rectangular barrier transmission probability](rectangular-barrier-transmission-probability.md)
2. [Finite rectangular barrier matching](finite-rectangular-barrier-matching.md)
3. [Quantum tunnelling](quantum-tunnelling.md)
4. [Potential barrier](potential-barrier.md)
5. [Quantum mechanics](quantum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Opaque barrier approximation](opaque-barrier-approximation.md)
