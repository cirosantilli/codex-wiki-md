<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take a constant infinitesimal [translation](../../../../translation-geometry.md) with fixed-coordinate [field variation](../../../../field-variation.md) $\delta\phi=\epsilon^\nu\partial_\nu\phi$. The associated change in the [Lagrangian density](../../../../lagrangian-density.md) is $\delta\mathcal L=\epsilon^\nu\partial_\nu\mathcal L=\partial_\mu(\epsilon^\nu\delta^\mu{}_{\nu}\mathcal L)$. Substituting this total derivative into the [Noether current](../../../../noether-current.md) gives $J^\mu=\epsilon^\nu T^\mu{}_{\nu}$, where

$$
\boxed{T^\mu{}_{\nu}=\partial^\mu\phi\,\partial_\nu\phi-\delta^\mu{}_{\nu}\left[\frac12\partial_\rho\phi\,\partial^\rho\phi-\frac12m^2\phi^2-\frac{\lambda}{24}\phi^4\right].}
$$

This is the [canonical stress-energy tensor](../../../../canonical-stress-energy-tensor.md). The chosen sign of the [translation](../../../../translation-geometry.md) parameter produces precisely this sign of the [Noether current](../../../../noether-current.md); reversing the parameter reverses the current without changing its conservation law.

To check [current conservation](../../../../conserved-current.md) directly, differentiate the [tensor](../../../../tensor.md). The terms containing $\partial_\nu\partial_\rho\phi$ cancel against the derivative of the [kinetic term](../../../../kinetic-term.md), leaving

$$
\partial_\mu T^\mu{}_{\nu}=
\left(\Box\phi+m^2\phi+\frac{\lambda}{6}\phi^3\right)\partial_\nu\phi
=F\partial_\nu\phi.
$$

Thus $\partial_\mu T^\mu{}_{\nu}=0$ [on shell](../../../../on-shell.md). Raising the second [Lorentz index](../../../../lorentz-index.md) gives $T^{\mu\nu}=T^{\nu\mu}$: this [scalar field](../../../../scalar-field.md) already has a symmetric [canonical stress-energy tensor](../../../../canonical-stress-energy-tensor.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
