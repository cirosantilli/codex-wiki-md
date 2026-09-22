<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Notation.** The source uses $p_s$ for both the hypothetical dry surface [pressure](../../../../pressure-split.md) and the actual surface [pressure](../../../../pressure-split.md) after [evaporation](../../../../evaporation.md). Distinguish them as $P_d$ and $P$, respectively, and interpret the specified [pressure](../../../../pressure-split.md) thickness $\Delta p$ as fixed. This conserves the original [hydrogen](../../../../hydrogen.md) inventory and permits $P$ to vary. Reading both occurrences as one fixed number would be inconsistent with adding [water vapor](../../../../water-vapor.md) to a closed [atmospheric column mass](../../../../atmospheric-column-mass.md) budget.

Let $E(T)$ denote the [saturation pressure](../../../../vapor-pressure.md) of [water](../../../../water.md), let $x$ be the [mole fraction](../../../../mole-fraction.md) of [water vapor](../../../../water-vapor.md) in the mixed layer, and let $M_d,M_v$ be the [molar masses](../../../../molar-mass.md) of [hydrogen](../../../../hydrogen.md) and [water](../../../../water.md). Surface [phase equilibrium](../../../../phase-equilibrium.md) and the [ideal gas law](../../../../ideal-gas-law.md) give

$$
x=\frac{E(T_s)}P,\qquad p_v(p)=xp.
$$

Because the layer has constant [temperature](../../../../temperature-split.md), its [relative humidity](../../../../relative-humidity.md) is

$$
\boxed{\mathrm{RH}(p)=\frac{p_v(p)}{E(T_s)}=\frac pP},\qquad P-\Delta p\leq p\leq P.
$$

Thus every level strictly above the surface is subsaturated: [hydrostatic balance](../../../../hydrostatic-balance.md) makes $p<P$, whereas the [saturation pressure](../../../../vapor-pressure.md) stays constant. The result does not require a dilute [water vapor](../../../../water-vapor.md) approximation.

The [Clausius-Clapeyron relation](../../../../clausius-clapeyron-relation.md), neglecting the [specific volume](../../../../specific-volume.md) of [liquid water](../../../../liquid-water.md) and treating the [water vapor](../../../../water-vapor.md) as an [ideal gas](../../../../ideal-gas-split.md), gives

$$
\frac{d\ln E}{dT}=\frac{L_v}{R_vT^2},\qquad
E(T)=E_t\exp\!\left[\frac{L_v}{R_v}\left(\frac1{T_t}-\frac1T\right)\right],\qquad R_v=\frac R{M_v}.
$$

Here $T_t,E_t$ are the [triple point](../../../../triple-point.md) values, $L_v$ is the specific [latent heat](../../../../latent-heat.md), and $R$ is the [molar gas constant](../../../../molar-gas-constant.md). All [temperatures](../../../../temperature-split.md) in these expressions are absolute. As throughout the question, this is a constant-[latent heat](../../../../latent-heat.md), [ideal gas](../../../../ideal-gas-split.md) model, not an extrapolation valid through the real [critical point](../../../../critical-point.md) of [water](../../../../water.md).

For a well-mixed [ideal gas](../../../../ideal-gas-split.md) mixture, its mean [molar mass](../../../../molar-mass.md) and [water vapor](../../../../water-vapor.md) [mass fraction](../../../../mass-fraction.md) are

$$
\overline M=M_d(1+ax),\qquad w_v=\frac{\epsilon x}{1+ax},\qquad
\epsilon=\frac{M_v}{M_d}\simeq9,\qquad a=\epsilon-1\simeq8.
$$

By [hydrostatic balance](../../../../hydrostatic-balance.md), the mixed layer has total [mass](../../../../mass.md) per unit area $\Delta p/g$, of which $w_v\Delta p/g$ is [water vapor](../../../../water-vapor.md). The remaining [atmosphere](../../../../atmosphere.md) contains no [water vapor](../../../../water-vapor.md). Consequently conservation of [hydrogen](../../../../hydrogen.md) [mass](../../../../mass.md) gives

$$
\frac P g=\frac{P_d}g+\frac{\Delta p}g w_v,
\qquad
P=P_d+\Delta p\frac{\epsilon E(T_s)}{P+aE(T_s)}.
$$

Equivalently the requested [quadratic equation](../../../../quadratic-equation.md) is

$$
\boxed{(P-P_d)(P+aE)=\epsilon\Delta p\,E.}
$$

For each $T_s$, calculate $E$, take the positive [root](../../../../root-of-a-root-system.md) of this [quadratic equation](../../../../quadratic-equation.md), and retain it only if $0\leq x<1$ and $P>\Delta p$. The last condition leaves a nonempty dry layer. In particular the dry constituent's surface [partial pressure](../../../../partial-pressure.md) is not generally $P_d$: $P_d$ measures its column weight, and the [hydrogen](../../../../hydrogen.md) and [water vapor](../../../../water-vapor.md) have different [molar masses](../../../../molar-mass.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
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
