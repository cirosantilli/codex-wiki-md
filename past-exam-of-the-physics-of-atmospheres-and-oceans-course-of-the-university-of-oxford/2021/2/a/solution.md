<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\kappa=R_d/c_p$, where $R_d$ is the [specific gas constant](../../../../specific-gas-constant.md) and $c_p$ the [specific heat capacity at constant pressure](../../../../specific-heat-capacity-at-constant-pressure.md). Conservation of [potential temperature](../../../../potential-temperature.md) on a dry [adiabatic process](../../../../adiabatic-process.md) gives

$$
T(p)=T_g\left(\frac p{p_s}\right)^\kappa,\qquad T_c=qT_g,\qquad q=\left(\frac{p_c}{p_s}\right)^\kappa.
$$

Let $Q=(1-\alpha_c)S$ be the absorbed stellar [irradiance](../../../../irradiance.md), and let $T_0=(Q/\sigma)^{1/4}$, with $\sigma$ the [Stefan-Boltzmann constant](../../../../stefan-boltzmann-constant.md). The transparent gas contributes no [thermal radiation](../../../../thermal-radiation.md). For a [cloud](../../../../cloud.md) with [emissivity](../../../../emissivity.md) $e$, [Kirchhoff's law of thermal radiation](../../../../kirchhoff-s-law-of-thermal-radiation.md) gives thermal absorptivity $e$; assume thermal transmissivity $1-e$ and negligible thermal reflection, as in the usual one-layer [grey body](../../../../grey-body.md) model. The outgoing [radiant flux](../../../../radiant-flux.md) is the transmitted surface emission plus upward [cloud](../../../../cloud.md) emission:

$$
Q=(1-e)\sigma T_g^4+e\sigma T_c^4.
$$

Thus

$$
\boxed{T_g=T_0\left[1-e+eq^4\right]^{-1/4},\qquad T_c=qT_g.}
$$

No factor of four is needed: $S$ is the incident [irradiance](../../../../irradiance.md) of the specified column, rather than a stellar-beam [irradiance](../../../../irradiance.md) that still needs a spherical average.

For fixed $\alpha_c,p_c,p_s$, increasing $e$ monotonically warms the ground when $0<q<1$. At $e=0$, $T_g=T_0$; at $e=1$, $T_c=T_0$ and $T_g=T_0/q$. A [cloud](../../../../cloud.md) at the surface, $q=1$, produces no such warming. Comparing with a genuinely cloud-free column also requires including its different [albedo](../../../../albedo.md): relative to $(S/\sigma)^{1/4}$, the ratio is $[(1-\alpha_c)/(1-e+eq^4)]^{1/4}$. Reflection can outweigh the [greenhouse effect](../../../../greenhouse-effect.md).

The governing balance here is the whole-column [radiation budget](../../../../radiation-budget.md). Imposing an additional purely radiative surface balance would incorrectly remove the [convective heat transfer](../../../../convective-heat-transfer.md) that the prescribed dry [adiabatic process](../../../../adiabatic-process.md) may require.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
