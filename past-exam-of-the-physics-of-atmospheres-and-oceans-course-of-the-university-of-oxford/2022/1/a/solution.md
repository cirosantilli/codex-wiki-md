<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [variable-latent-heat saturation curve](../../../../variable-latent-heat-saturation-curve.md) of a pure saturated [water](../../../../water.md) [atmosphere](../../../../atmosphere.md), the total [pressure](../../../../pressure-split.md) equals the [saturation pressure](../../../../vapor-pressure.md). The exact [Clausius-Clapeyron relation](../../../../clausius-clapeyron-relation.md) along the [phase coexistence curve](../../../../phase-coexistence-curve.md) is

$$
\frac{dp}{dT}=\frac{L(T)}{T(v_v-v_c)},
$$

where $v_v,v_c$ are the specific volumes of the [vapor](../../../../vapor.md) and condensed [thermodynamic phase](../../../../thermodynamic-phase.md). Neglecting $v_c$ and using the [ideal gas law](../../../../ideal-gas-law.md), $v_v=R_{\rm wv}T/p$, gives

$$
\frac{d\ln p}{dT}=\frac{L(T)}{R_{\rm wv}T^2},\qquad
\ln\frac p{p_*}=\int_{T_*}^{T}\frac{L(\theta)}{R_{\rm wv}\theta^2}\,d\theta.
$$

The [triple point](../../../../triple-point.md) provides the integration constant. Below it, the prescribed [latent heat](../../../../latent-heat.md) is constant, so

$$
\boxed{\ln\frac p{p_*}=\frac{L_s}{R_{\rm wv}}\left(\frac1{T_*}-\frac1T\right),\quad T\leq T_*.}
$$

Above it, write $K=L_*/[R_{\rm wv}(T_c-T_*)]$. Integrating $K(T_c/T^2-1/T)$ gives

$$
\boxed{\ln\frac p{p_*}=K\left[T_c\left(\frac1{T_*}-\frac1T\right)-\ln\frac{T}{T_*}\right],\quad T_*\leq T<T_c.}
$$

These are the requested implicit [temperature](../../../../temperature-split.md) profiles $T(p)$. Both branches meet at $(T_*,p_*)$, and each is monotone before the limiting [liquid-gas critical point](../../../../liquid-gas-critical-point.md). The lower branch describes equilibrium with [ice](../../../../ice.md), rather than a stable [liquid](../../../../liquid.md) surface. A stable [liquid](../../../../liquid.md) [ocean](../../../../ocean.md) surface belongs to the upper branch; the colder upper [atmosphere](../../../../atmosphere.md) may use the lower branch. [Hydrostatic balance](../../../../hydrostatic-balance.md) is needed to convert this relation into a height profile, but not to obtain $T(p)$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
