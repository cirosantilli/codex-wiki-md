<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $R_A,R_B$ be the specific [specific gas constants](../../../../specific-gas-constant.md) and $c_{pA},c_{pB}$ the specific [heat capacities](../../../../heat-capacity.md) of the noncondensible gas and vapour. Write $e_s(T)$ for the [saturation vapor pressure](../../../../saturation-vapor-pressure.md), $r$ for vapour [mass](../../../../mass.md) per unit dry-gas [mass](../../../../mass.md), and $\epsilon=R_A/R_B$. For a dilute [ideal gas](../../../../ideal-gas-split.md) mixture,

$$
r=\frac{\epsilon e_s}{p-e_s}\simeq\epsilon\frac{e_s}p,\qquad
\frac{d\ln e_s}{dT}=\frac{L}{R_BT^2}.
$$

The second equation is the [Clausius-Clapeyron equation](../../../../clausius-clapeyron-relation.md), neglecting condensed-phase volume and taking constant [latent heat](../../../../latent-heat.md) $L$. The [first law of thermodynamics](../../../../first-law-of-thermodynamics-split.md) for saturated ascent, with condensate removed and negligible condensate heat capacity, is to leading order

$$
c_{pA}\,dT-R_AT\,d\ln p=-L\,dr.
$$

Since $dr=r[L\,dT/(R_BT^2)-d\ln p]$, the resulting [moist adiabat](../../../../moist-adiabat.md) has logarithmic slope

$$
\frac{d\ln T}{d\ln p}=\frac{R_A}{c_{pA}}\frac{1+Lr/(R_AT)}{1+L^2r/(c_{pA}R_BT^2)}.
$$

Consequently a sufficient [dry adiabat](../../../../dry-adiabat.md) criterion is

$$
\boxed{\frac{e_s}p\ll1,\quad \frac{r c_{pB}}{c_{pA}}\ll1,\quad\frac{Lr}{R_AT}\ll1,\quad\frac{L^2r}{c_{pA}R_BT^2}\ll1.}
$$

The first two conditions justify neglecting the vapour's effects on the gas law and sensible [heat capacity](../../../../heat-capacity.md); the last two suppress latent heating. With $x=R_A/c_{pA}$ and $\beta=L/(R_BT)$, the latent conditions are $\beta e_s/p\ll1$ and $x\beta^2e_s/p\ll1$. Usually $x\beta\gg1$, so the squared-latent term gives the stronger condition. At sufficiently low [surface temperature](../../../../surface-temperature.md), the exponential smallness of $e_s(T_s)$ makes these conditions hold and

$$
\boxed{T(p)\simeq T_s(p/p_s)^x.}
$$

These are local conditions along the column. They can be checked at the surface when $x\beta_s>1+2x$: on this dry profile the strongest latent parameter is proportional to $\exp[(1+2x)\zeta-\beta_s(e^{x\zeta}-1)]$ and decreases upwards. Without that restriction a surface-only test need not bound every altitude. If suspended condensate is retained, its own [heat capacity](../../../../heat-capacity.md) and loading must also be negligible; saturation alone does not specify those quantities.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
