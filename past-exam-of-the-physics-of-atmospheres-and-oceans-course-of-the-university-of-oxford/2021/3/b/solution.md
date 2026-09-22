<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $e_v$ be the parcel's [water vapor](../../../../water-vapor.md) [partial pressure](../../../../partial-pressure.md). Fixed [mole fraction](../../../../mole-fraction.md) before [condensation](../../../../condensation.md) means $e_v/p$ is constant. Its [dew point](../../../../dew-point.md) $T_D$ is defined by $E(T_D)=e_v$, where $E$ is the [saturation pressure](../../../../vapor-pressure.md). The [Clausius-Clapeyron relation](../../../../clausius-clapeyron-relation.md) gives

$$
\frac{L_v}{R_vT_D^2}\frac{dT_D}{dz}=\frac{d\ln e_v}{dz}=\frac{d\ln p}{dz}
\simeq-\frac g{R_d T}.
$$

The last approximation uses [hydrostatic balance](../../../../hydrostatic-balance.md), the [ideal gas law](../../../../ideal-gas-law.md), and an environmental [temperature](../../../../temperature-split.md) close to the parcel's. Rearrangement yields

$$
\frac{d\ln T_D}{dz}=-\frac{gR_v}{L_vR_d}\frac{T_D}{T}.
$$

For a modest initial [dew-point depression](../../../../dew-point-depression.md), $T_D/T\simeq1$ in absolute [temperature](../../../../temperature-split.md), so

$$
\boxed{T_D(z)\simeq T_{D,s}e^{-z/H},\qquad H=\frac{L_vR_d}{gR_v}.}
$$

With $L_v\simeq2.5\times10^6\,\mathrm{J\,kg^{-1}}$, $R_d\simeq287\,\mathrm{J\,kg^{-1}\,K^{-1}}$, and $R_v\simeq461.5\,\mathrm{J\,kg^{-1}\,K^{-1}}$, $H\simeq1.58\times10^5\,\mathrm m$. This [dew point](../../../../dew-point.md) scale is much longer than the atmospheric [pressure scale height](../../../../pressure-scale-height.md).

The [exponential function](../../../../exponential-function.md) is an approximation, not the exact consequence of a dry [adiabatic process](../../../../adiabatic-process.md). Retaining $T=T_s-\Gamma_d z$ gives $p/p_s=(T/T_s)^{c_p/R_d}$ and the useful comparison

$$
\frac1{T_D(z)}=\frac1{T_{D,s}}-\frac{R_v}{L_v}\frac{c_p}{R_d}\ln\!\frac{T(z)}{T_s}.
$$

It also shows explicitly that expansion lowers the [dew point](../../../../dew-point.md) even before any [water vapor](../../../../water-vapor.md) condenses.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
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
