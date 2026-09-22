<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A convenient parameter is the [water vapor](../../../../water-vapor.md) [mole fraction](../../../../mole-fraction.md) itself. The [mass conservation](../../../../mass-conservation.md) calculation yields

$$
P(x)=P_d+\frac{\epsilon\Delta p\,x}{1+ax},\qquad E(x)=xP(x).
$$

Both functions increase for $0\leq x\leq1$. At the endpoint,

$$
P(1)=E(1)=P_d+\Delta p.
$$

Therefore the physically admissible [hydrogen](../../../../hydrogen.md)–[water vapor](../../../../water-vapor.md) mixture requires

$$
\boxed{E(T_s)<P_d+\Delta p.}
$$

Beyond this bound, the formal positive [quadratic equation](../../../../quadratic-equation.md) [root](../../../../root-of-a-root-system.md) requires $x>1$, equivalently a negative [hydrogen](../../../../hydrogen.md) [partial pressure](../../../../partial-pressure.md). It is the physical constraints, rather than loss of real [roots](../../../../root-of-a-root-system.md), that end the solution branch. For a concrete example, put $P_d=\Delta p=1$ in consistent [pressure](../../../../pressure-split.md) units, $\epsilon=9$, and $E=3$. The positive [root](../../../../root-of-a-root-system.md) of $P^2+23P-51=0$ is about $2.037$, giving $x\simeq1.473$, which is impossible.

The limiting [temperature](../../../../temperature-split.md) is obtained from $E(T_*)=P_d+\Delta p$:

$$
\frac1{T_*}=\frac1{T_t}-\frac{R_v}{L_v}\ln\!\frac{P_d+\Delta p}{E_t}.
$$

This finite limit exists above $T_t$ if $E_t<P_d+\Delta p<E_t\exp[L_v/(R_vT_t)]$. The upper qualification matters mathematically: the stipulated constant-[latent heat](../../../../latent-heat.md) formula has a finite limiting [saturation pressure](../../../../vapor-pressure.md) as $T\to\infty$, so for an arbitrarily large unspecified $P_d+\Delta p$ the printed assertion of a finite breakdown [temperature](../../../../temperature-split.md) is not unconditional. For a concrete formal counterexample, choose $P_d+\Delta p=10^{15}\,\mathrm{Pa}$: with the usual triple-point constants the model has $E(\infty)\simeq2.5\times10^{11}\,\mathrm{Pa}$, so it never reaches the proposed inventory limit. This is a counterexample inside the stipulated equations, not a physically credible high-[pressure](../../../../pressure-split.md) [ideal gas](../../../../ideal-gas-split.md) ocean. Actual [liquid water](../../../../liquid-water.md) also ceases to exist above its [critical point](../../../../critical-point.md), before such an extrapolation would make sense.

Physically, the imposed finite-[pressure](../../../../pressure-split.md)-thickness layer can hold no more than $\Delta p/g$ of [water vapor](../../../../water-vapor.md) per unit area. As $x\to1$, it expels all its [hydrogen](../../../../hydrogen.md) into the dry upper layer. A still larger surface [saturation pressure](../../../../vapor-pressure.md) cannot coexist with this geometry. The layer must deepen, the [temperature](../../../../temperature-split.md) profile must change, or the assumed [phase equilibrium](../../../../phase-equilibrium.md) must fail. If $P_d<\Delta p$, the additional restriction $P>\Delta p$ can also exclude the low-[temperature](../../../../temperature-split.md) end of the branch.

## ↑ Ancestors (12)

1. [B](../b.md)
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
