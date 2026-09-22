# Franck-Hertz energy-loss model

↑ **Parent:** [Franck-Hertz experiment](franck-hertz-experiment.md)

A useful [Franck-Hertz energy-loss model](franck-hertz-energy-loss-model.md) separates three operations: accelerating an [electron](electron.md), losing a discrete [energy](energy-split.md) $\Delta$ in an [inelastic collision](inelastic-collision.md), and selecting the surviving [electrons](electron.md) with a retarding collector. The collector measures an accepted fraction of an outgoing [energy](energy-split.md) distribution. This makes the experiment a small [inverse problem](inverse-problem-split.md): the [electric current](electric-current.md) depends on both the collision physics and the readout.

For a deliberately simple one-channel model, let $u\geq0$ be the incoming [kinetic energy](kinetic-energy.md), and let $p(u)$ be the [probability](probability.md) that one encounter excites the [chemical atom](atom-physics.md). Set $p(u)=0$ for $u<\Delta$ and $0\leq p(u)\leq1$ otherwise. The conditional [probability distribution](probability-distribution-split.md) of outgoing [kinetic energy](kinetic-energy.md) $E$ is the discrete loss kernel

$$
K(E\mid u)=[1-p(u)]\delta(E-u)+p(u)\delta(E-u+\Delta).
$$

Here $\delta$ is the [Dirac delta function](dirac-delta-function.md). The kernel has unit [integral](integral-split.md), no negative outgoing [energy](energy-split.md), and mean outgoing [kinetic energy](kinetic-energy.md) $u-p(u)\Delta$. It neglects the small recoil loss in an [elastic collision](elastic-collision.md), other excitation channels and [ionization](ionization.md). The threshold permits excitation; it does not require $p(u)=1$ above threshold. In particular, choosing a single $\Delta=4.9\,\mathrm{eV}$ here isolates the characteristic channel discussed above without claiming it is mercury's lowest possible excitation.

**Table of contents**

- [Franck-Hertz retarding collector transfer](franck-hertz-retarding-collector-transfer.md)
- [Franck-Hertz repeated-loss collection model](franck-hertz-repeated-loss-collection-model.md)
- [Franck-Hertz spacing fit and contact offset](franck-hertz-spacing-fit-and-contact-offset.md)

## ↑ Ancestors (7)

1. [Franck-Hertz experiment](franck-hertz-experiment.md)
2. [Excited state](excited-state.md)
3. [Energy eigenvalue](energy-eigenvalue-split.md)
4. [Quantum mechanics](quantum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Franck-Hertz energy-loss model](franck-hertz-energy-loss-model.md)
- [Franck-Hertz retarding collector transfer](franck-hertz-retarding-collector-transfer.md)
