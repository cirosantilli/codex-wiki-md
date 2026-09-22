<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $z$ to increase inward, so the positive coefficient $A$ describes an inward-increasing [temperature](../../../../../../temperature.md). Constant gravity and [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) give $dP/dz=\rho g$, hence

$$
\frac{dT}{dP}=\frac{A}{gT^3},\qquad \nabla_{\rm rad}=\frac{AP}{gT^4}.
$$

Matching the [radiative temperature gradient](../../../../../../radiative-temperature-gradient.md) to the [adiabatic temperature gradient](../../../../../../adiabatic-temperature-gradient.md) gives the formal local boundary relation

$$
\boxed{P_b=\frac{g}{A}\nabla_{\rm ad}T_b^4}.
$$

The same result follows from [radiative diffusion](../../../../../../radiative-diffusion.md): for constant upward thermal flux $F$ and [Rosseland mean opacity](../../../../../../rosseland-mean-opacity.md) $\kappa$, $A=3\kappa F/(16\sigma_{\rm SB})$.

There is an important limitation to treating $A$ as constant over the entire radiative layer. Integration from an irradiated outer boundary gives

$$
T^4=T_0^4+\frac{4A}{g}P,\qquad \nabla_{\rm rad}=\frac14\left(1-\frac{T_0^4}{T^4}\right)<\frac14.
$$

For a diatomic [ideal gas](../../../../../../ideal-gas.md), $\nabla_{\rm ad}=2/7>1/4$, so this profile cannot actually reach a [radiative-convective boundary](../../../../../../radiative-convective-boundary.md). Formally, imposing a constant $\nabla_{\rm ad}$ would give

$$
P_b=\frac{gT_0^4}{A}\frac{\nabla_{\rm ad}}{1-4\nabla_{\rm ad}},
$$

which is positive only for $0<\nabla_{\rm ad}<1/4$. **A finite boundary for a normal molecular atmosphere requires additional [opacity](../../../../../../opacity.md), flux, or thermodynamic variation.** The local matching formula is usable near a real boundary, but constant $A$ is not a complete global model of it. This is the [convective stability of a constant-opacity irradiated atmosphere](../../../../../../convective-stability-of-a-constant-opacity-irradiated-atmosphere.md).

For the intended order-of-magnitude scaling, suppose the local values of $g/A$ and $\nabla_{\rm ad}$ are comparable for [Jupiter](../../../../../../jupiter.md) and a [hot Jupiter](../../../../../../hot-jupiter.md), and assume $T_b$ scales with [planetary equilibrium temperature](../../../../../../planetary-equilibrium-temperature.md). Equal absorbed-flux factors around the same stellar luminosity give $T_b\propto a^{-1/2}$. Taking $a_J=5.2\,\mathrm{AU}$ and a representative close-in orbit $a_h=0.05\,\mathrm{AU}$ yields

$$
\frac{P_{b,h}}{P_{b,J}}\sim\left(\frac{T_{b,h}}{T_{b,J}}\right)^4\sim\left(\frac{5.2}{0.05}\right)^2,
\qquad \boxed{P_{b,h}\sim10^3\,\mathrm{bar}}.
$$

This illustrates how irradiation can push a boundary much deeper. It is a conditional estimate calibrated from the supplied $0.1\,\mathrm{bar}$ reference, not a self-consistent prediction of the globally constant-$A$ model. Different intrinsic cooling flux, [opacity](../../../../../../opacity.md), gravity, or [atmospheric metallicity of a giant planet](../../../../../../atmospheric-metallicity-of-a-giant-planet.md) can substantially alter it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
