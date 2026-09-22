# Population inversion

↑ **Parent:** [Stimulated emission](stimulated-emission.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Population_inversion)

A [population inversion](population-inversion.md) puts more emitters in the upper than in the lower [quantum state](quantum-state.md) of a transition in the nondegenerate two-level model. Let $N_2,N_1$ be their number densities. Equal stimulated-transition strengths make the emission rate proportional to $N_2$ and the competing [photon absorption](photon-absorption.md) rate proportional to $N_1$, so net [optical gain](optical-gain.md) is proportional to $N_2-N_1$. For $N_2=6\times10^{20}\,\mathrm{m^{-3}}$ and $N_1=4\times10^{20}\,\mathrm{m^{-3}}$, the difference is positive; swapping them makes the medium absorb. Equal populations give zero net stimulated contribution. With degenerate levels, the relevant comparison uses populations per [statistical weight of an atomic level](statistical-weight-of-an-atomic-level.md), rather than simply $N_2>N_1$.

Why pump through extra levels? Ordinary steady resonant pumping of a nondegenerate two-level system drives both [photon absorption](photon-absorption.md) and [stimulated emission](stimulated-emission.md). With equal induced rate $W$ and upper-state decay rate $\Gamma$, its elementary population equation is

$$
\dot N_2=W(N_1-N_2)-\Gamma N_2,
\qquad
\frac{N_2}{N_1}=\frac{W}{W+\Gamma}\leq1
$$

at a stationary population. Increasing this pump saturates towards $N_2=N_1$; it cannot sustain [population inversion](population-inversion.md) in this model. This is a steady rate-equation conclusion, not a universal prohibition on all driven two-level dynamics or all possible [laser](laser.md) gain mechanisms. [Franz Kärtner, MIT 6.974, Chapter 6, §§6.7–6.8: saturation and rate equations](https://ocw.mit.edu/courses/6-974-fundamentals-of-photonics-quantum-electronics-spring-2006/2641db6431ea70989c29e8512d5d91a7_chapter6.pdf).

In a familiar three-level path, pumping excites a higher level which relaxes into the upper lasing level; the lower lasing level is the ground state, so substantial ground-state depletion is needed. A four-level path also provides rapid emptying of the lower lasing level into a separate ground state. Suitable lifetimes then allow accumulation above and depletion below the lasing transition. Pumping still supplies the [energy](energy.md): extra levels provide a route to [population inversion](population-inversion.md), not free [energy](energy.md). [Franz Kärtner, MIT 6.974, §7.2.1: three- and four-level laser media](https://ocw.mit.edu/courses/6-974-fundamentals-of-photonics-quantum-electronics-spring-2006/18f30fad63a62ef4dd894d3752b55a60_chapter7.pdf).

## ↑ Ancestors (6)

1. [Stimulated emission](stimulated-emission.md)
2. [Laser](laser.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Laser](laser.md)
- [Laser threshold](laser-threshold.md)
- [Optical gain](optical-gain.md)
- [Population inversion](population-inversion.md)
