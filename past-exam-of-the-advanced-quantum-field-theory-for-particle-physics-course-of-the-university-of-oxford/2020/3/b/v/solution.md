<h1 id="3/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

There are four [tree-level Feynman diagrams](../../../../../tree-level-feynman-diagram.md): three [photon](../../../../../photon.md) exchange graphs with pairings $12|34$, $13|24$, $14|23$, and the four-photon [contact interaction](../../../../../contact-interaction-quantum-mechanics.md). They are drawn in the bottom row of the figure. With no external [fermions](../../../../../fermion.md) or [Faddeev-Popov ghost fields](../../../../../faddeev-popov-ghost.md), an internal matter or ghost line would have to close into a loop; it cannot add a [tree-level Feynman diagram](../../../../../tree-level-feynman-diagram.md) here.

Use all-incoming null [four-momenta](../../../../../four-momentum.md) $k_i$ with $\sum_i k_i=0$. Let $\varepsilon_i$ be the external [photon polarization vectors](../../../../../photon-polarization-vector.md), including the complex conjugation for physical outgoing [photons](../../../../../photon.md), and impose $k_i\cdot\varepsilon_i=0$. For one pairing $ij|kl$, put $K=k_i+k_j=-(k_k+k_l)$. At the first cubic [Feynman vertex](../../../../../interaction-vertex.md), the terms proportional to $k_i\cdot\varepsilon_i$ and $k_j\cdot\varepsilon_j$ vanish, leaving

$$
\varepsilon_{i\alpha}\varepsilon_{j\beta}V_3^{\alpha\beta\rho}(k_i,k_j,-K)=-2\lambda(\varepsilon_i\cdot\varepsilon_j)K^\rho.
$$

At the other end, the incoming internal [four-momentum](../../../../../four-momentum.md) is $+K$, giving $+2\lambda(\varepsilon_k\cdot\varepsilon_l)K^\sigma$. The [Feynman gauge](../../../../../feynman-gauge.md) [photon propagator](../../../../../photon-propagator.md) then gives

$$
i\mathcal M_{ij|kl}=(-2\lambda)(2\lambda)(\varepsilon_i\cdot\varepsilon_j)(\varepsilon_k\cdot\varepsilon_l)K^\rho\frac{-ig_{\rho\sigma}}{K^2+i0}K^\sigma
=4i\lambda^2(\varepsilon_i\cdot\varepsilon_j)(\varepsilon_k\cdot\varepsilon_l).
$$

The last expression is evaluated at generic kinematics, with singular channel limits taken after cancellation. Summing the three pairings produces $+4i\lambda^2P$, where

$$
P=(\varepsilon_1\cdot\varepsilon_2)(\varepsilon_3\cdot\varepsilon_4)+(\varepsilon_1\cdot\varepsilon_3)(\varepsilon_2\cdot\varepsilon_4)+(\varepsilon_1\cdot\varepsilon_4)(\varepsilon_2\cdot\varepsilon_3).
$$

The quartic [Feynman vertex](../../../../../interaction-vertex.md) contributes $i\mathcal M_{\mathrm{contact}}=-4i\lambda^2P$. Thus

$$
\boxed{i\mathcal M_{\mathrm{tree}}=4i\lambda^2P-4i\lambda^2P=0.}
$$

This is the [tree photon-scattering cancellation in a quadratic Abelian gauge](../../../../../tree-photon-scattering-cancellation-in-a-quadratic-abelian-gauge.md): the individual [gauge fixing](../../../../../gauge-fixing.md) interactions cancel in the physical [scattering amplitude](../../../../../scattering-amplitude.md). The argument uses transverse external [photon polarization vectors](../../../../../photon-polarization-vector.md); it does not assert that an arbitrary [off shell](../../../../../off-shell.md) four-point [correlation function](../../../../../correlation-function.md) vanishes. Physical [light-by-light scattering](../../../../../light-by-light-scattering.md) first occurs through charged-particle [loop Feynman diagrams](../../../../../loop-feynman-diagram.md).

## ↑ Ancestors (13)

1. [V](../v.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2020](../../../../2020-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
