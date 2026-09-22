<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Rename the [Antoine equation](../../../../antoine-equation.md) coefficients $A_A,B_A,C_A$ to distinguish them from the heat-capacity constants. The logarithmic slope is independent of the [pressure](../../../../pressure-split.md) unit:

$$
\frac{d\ln p_{\rm sat}}{dT}=\ln(10)\frac{B_A}{(T+C_A)^2}.
$$

Using an ideal vapour and neglecting liquid specific volume, Clausius–Clapeyron gives $d\ln p_{\rm sat}/dT=L_v/(R_vT^2)$. Therefore the positive magnitude of the [latent heat](../../../../latent-heat.md) released on [condensation](../../../../condensation.md) is

$$
\boxed{L_v(T)=R_v\ln(10)B_A\left(\frac{T}{T+C_A}\right)^2.}
$$

For $C_A=-198.043\,\mathrm K$, $d\ln L_v/dT=2C_A/[T(T+C_A)]<0$ over the quoted range. With $R_v\simeq461.5\,\mathrm{J\,kg^{-1}\,K^{-1}}$, this fit implies approximately $2.984\,\mathrm{MJ\,kg^{-1}}$ at $380\,\mathrm K$ and $1.598\,\mathrm{MJ\,kg^{-1}}$ at $573\,\mathrm K$. The required ratio does not depend on $R_v$:

$$
\boxed{\frac{L_v(573)}{L_v(380)}=
\left[\frac{573(380-198.043)}{380(573-198.043)}\right]^2\simeq0.5354.}
$$

The decreasing trend is qualitatively consistent with the liquid and vapour phases becoming less distinct towards the [liquid-gas critical point](../../../../liquid-gas-critical-point.md). However, the full Clapeyron relation is $L_v=T(v_v-v_l)\,dp_{\rm sat}/dT$: at criticality the two specific volumes merge and the [latent heat](../../../../latent-heat.md) vanishes. Neglecting $v_l$ and treating the vapour as ideal then fail. The Antoine coefficients are not licensed for extrapolation beyond $573\,\mathrm K$, and [derivatives](../../../../derivative.md) of an approximate [pressure](../../../../pressure-split.md) fit can be less accurate than the fitted [pressures](../../../../pressure-split.md) themselves.

A concrete check exposes the extrapolation failure: at the supplied $647\,\mathrm K$ critical [temperature](../../../../temperature-split.md) the formula would still give $L_v\simeq1.42\,\mathrm{MJ\,kg^{-1}}$, rather than zero, and $p_{\rm sat}\simeq134\,\mathrm{bar}$ rather than $221\,\mathrm{bar}$. Above the true [liquid-gas critical point](../../../../liquid-gas-critical-point.md) there is no liquid–vapour coexistence curve or [condensation](../../../../condensation.md) [latent heat](../../../../latent-heat.md) in the same sense. The last panel of the original figure in [solution](../b/solution.md) makes this limitation visible.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
