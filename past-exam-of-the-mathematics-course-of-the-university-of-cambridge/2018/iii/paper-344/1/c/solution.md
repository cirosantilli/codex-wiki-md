<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At [thermal equilibrium](../../../../../../thermal-equilibrium.md), [microscopic reversibility](../../../../../../microscopic-reversibility.md) equates the probabilities of a path and its reversed path when both include their [Boltzmann distribution](../../../../../../boltzmann-distribution.md) initial weights. Denote their endpoint states by $z_1,z_2$, including velocity if needed. Since the [Hamiltonian](../../../../../../hamiltonian.md) is even under [time reversal in classical mechanics](../../../../../../time-reversal-in-classical-mechanics.md),

$$
\rho_{\rm eq}(z_1)\mathbb P_F
=\rho_{\rm eq}(z_2)\mathbb P_B,
\qquad \rho_{\rm eq}(z)\propto e^{-\beta H(z)},
\qquad \beta=\frac1{k_BT}.
$$

This [detailed balance](../../../../../../detailed-balance.md) condition and the [energy balance for an autonomous Lagrangian](../../../../../../energy-balance-for-an-autonomous-lagrangian.md) yield

$$
\frac{\mathbb P_F}{\mathbb P_B}=e^{-\beta(H_2-H_1)},
\qquad \frac{2\zeta}{\sigma^2}=\beta,
\qquad \boxed{\sigma^2=2\zeta k_BT}.
$$

This is the [fluctuation-dissipation relation for a Langevin particle](../../../../../../fluctuation-dissipation-relation-for-a-langevin-particle.md): the strength of [Gaussian white noise](../../../../../../gaussian-white-noise.md) is fixed by the damping and [temperature](../../../../../../temperature.md), with $k_B$ the [Boltzmann constant](../../../../../../boltzmann-constant.md).

For an equilibrium [coarse-grained variable](../../../../../../coarse-grained-variable.md), the unresolved microscopic states contribute [entropy](../../../../../../entropy.md); their statistical weight is encoded in the [Helmholtz free energy](../../../../../../helmholtz-free-energy.md), rather than in a single microscopic energy. Relative to the same reference measure, $\rho_{\rm eq}(x)\propto e^{-\beta F(x)}$, so [microscopic reversibility](../../../../../../microscopic-reversibility.md) becomes

$$
\boxed{\frac{\mathbb P_F}{\mathbb P_B}=e^{-\beta(F_2-F_1)}}.
$$

This extension assumes an equilibrium coarse-grained description with reversible path statistics; externally driven dynamics need not obey this relation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
