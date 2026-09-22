# Catalytic barriers and reaction free energy

↑ **Parent:** [Catalysis](catalysis.md)

A directional [Gibbs energy of activation](gibbs-energy-of-activation.md) measures the climb from a starting state to a [transition state](transition-state.md). The net standard reaction change in [Gibbs free energy](gibbs-free-energy.md) measures the difference between endpoints. Changing the climb can strongly change a [rate constant](rate-constant.md) while leaving that endpoint difference intact. For two illustrative single-barrier routes with common endpoint levels $G_{\mathrm A}^\circ$ and $G_{\mathrm B}^\circ$,

$$
\Delta G_f^{\ddagger\circ}=G_{\mathrm{TS}}^\circ-G_{\mathrm A}^\circ,
\qquad
\Delta G_r^{\ddagger\circ}=G_{\mathrm{TS}}^\circ-G_{\mathrm B}^\circ,
\qquad
\Delta G_f^{\ddagger\circ}-\Delta G_r^{\ddagger\circ}=\Delta_rG^\circ.
$$

Lowering the common [transition state](transition-state.md) level lowers both directional [Gibbs energies of activation](gibbs-energy-of-activation.md); it does not lower just the forward climb. The usual statement that a [catalyst](catalyst.md) lowers an [activation energy](activation-energy.md) describes a kinetic route, not a change in the net [Gibbs free energy](gibbs-free-energy.md). An [activation energy](activation-energy.md) inferred from an [Arrhenius plot](arrhenius-plot.md) is also distinct from a [Gibbs energy of activation](gibbs-energy-of-activation.md) at one [temperature](temperature.md).

<a id="image-catalysis-barriers-and-net-free-energy"></a>
![](catalysis-barriers-and-net-free-energy.png)

**[Figure 57](#image-catalysis-barriers-and-net-free-energy). Illustrative catalysis schematic: different barriers, identical endpoint Gibbs free energy difference**. Chosen levels in $\mathrm{kJ\,mol^{-1}}$: A plus regenerated C at $0$, B plus regenerated C at $-3$, and schematic maxima at $12$ and $7$. Forward barriers are $12$ and $7$; reverse barriers are $15$ and $10$. Neither curve is a measured molecular path. The [reaction coordinate](reaction-coordinate.md) is not time. These values illustrate the barrier bookkeeping and do not parametrize the separate [reversible catalytic relaxation](reversible-catalytic-relaxation.md) example.

With a common prefactor in [transition state theory](transition-state-theory.md), subtracting the directional barriers yields

$$
\frac{k_f}{k_r}=\exp\!\left(-\frac{\Delta_rG^\circ}{RT}\right)=K,
$$

where $R$ is the [molar gas constant](molar-gas-constant.md) and $T$ is the absolute [temperature](temperature.md). This particular [rate constant](rate-constant.md) ratio requires the simple compatible directional [rate laws](rate-law.md) and consistent [standard states](standard-state.md); a general multistep [reaction mechanism](reaction-mechanism.md) does not supply two arbitrary measured [rate constants](rate-constant.md) whose ratio must equal $K$. At fixed [temperature](temperature.md) a [catalyst](catalyst.md) preserves $K$ for the same net conversion. The actual reaction change in [Gibbs free energy](gibbs-free-energy.md), $\Delta_rG=\Delta_rG^\circ+RT\ln Q$, is likewise unchanged at the same [reaction quotient](reaction-quotient.md) $Q$. Composition changes during the faster approach to [chemical equilibrium](chemical-equilibrium.md), so comparing mixtures at the same elapsed time need not compare the same $Q$.[§13.3, Effect of a Catalyst: both directional rates accelerate while equilibrium composition is unchanged](chemistry-2e-by-paul-flowers-and-others/13-3-shifting-equilibria-le-chatelier%E2%80%99s-principle.md)

## ↑ Ancestors (5)

1. [Catalysis](catalysis.md)
2. [Chemical kinetics](chemical-kinetics.md)
3. [Chemical reaction](chemical-reaction.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)
