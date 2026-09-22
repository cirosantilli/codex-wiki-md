# Joule-Thomson coefficient

↑ **Parent:** [Enthalpy](enthalpy-split.md)

The [Joule-Thomson coefficient](joule-thomson-coefficient.md) is the local [temperature](temperature-split.md) response to changing [pressure](pressure-split.md) at fixed [enthalpy](enthalpy-split.md) and fixed amount and composition:

$$
\mu_{\rm JT}=\left(\frac{\partial T}{\partial p}\right)_H,
\qquad [\mu_{\rm JT}]=\mathrm{K\,Pa^{-1}}.
$$

It describes the equilibrium endpoints of a [Joule-Thomson effect](joule-thomson-effect.md) experiment meeting the [steady-flow energy balance](steady-flow-energy-balance.md) assumptions. With $\Delta p=p_2-p_1<0$, a sufficiently small drop gives $\Delta T\simeq\mu_{\rm JT}\Delta p$. Thus $\mu_{\rm JT}>0$ means cooling, $\mu_{\rm JT}<0$ warming, and $\mu_{\rm JT}=0$ no first-order change. At zero coefficient, a finite drop can still change [temperature](temperature-split.md). For a chosen illustrative local value $\mu_{\rm JT}=0.20\,\mathrm{K\,bar^{-1}}$ and $\Delta p=-0.50\,\mathrm{bar}$, the linear prediction is $\Delta T=-0.10\,\mathrm K$; these are stipulated numbers, not measured gas properties.

For a fixed-composition [simple compressible system](simple-compressible-system.md), the measurable form is

$$
\mu_{\rm JT}
=\frac{T(\partial V/\partial T)_p-V}{C_p}
=\frac{V}{C_p}(T\alpha-1).
$$

Here $C_p$ is the whole sample's [heat capacity at constant pressure](heat-capacity-at-constant-pressure.md) and $\alpha$ its volumetric [coefficient of thermal expansion](coefficient-of-thermal-expansion.md); alternatively use [molar volume](molar-volume.md) and [molar heat capacity](molar-heat-capacity.md) consistently. An [ideal gas](ideal-gas-split.md) has $\alpha=1/T$, so $\mu_{\rm JT}=0$. Its [enthalpy](enthalpy-split.md) depends only on [temperature](temperature-split.md); positive [heat capacity at constant pressure](heat-capacity-at-constant-pressure.md) then makes any such finite throttle preserve [temperature](temperature-split.md). A [real gas](real-gas.md) can have either sign. For $C_p>0$, compare $T\alpha$ with one: the [thermal expansion](thermal-expansion.md) response decides the sign, not insulation alone.[Fitzpatrick, Joule-Thompson Throttling, equations 6.175–6.182: ideal-gas limit and coefficient](thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/joule-thompson-throttling.md)

A short derivation uses $dH=T\,dS+V\,dp$ and the [Maxwell relation](maxwell-relations.md) $(\partial S/\partial p)_T=-(\partial V/\partial T)_p$:

$$
dH=C_p\,dT+\left[V-T\left(\frac{\partial V}{\partial T}\right)_p\right]dp.
$$

Setting $dH=0$ gives the coefficient. These are equilibrium [state function](state-function.md) identities, not a claim of a [reversible thermodynamic process](reversible-thermodynamic-process.md) inside the throttle. For a finite drop, solve the endpoint [enthalpy](enthalpy-split.md) equality or integrate

$$
T_2-T_1=\int_{p_1}^{p_2}\mu_{\rm JT}(T(p),p)\,dp
$$

along the constant-[enthalpy](enthalpy-split.md) equilibrium curve. The coefficient can change sign during that integration, as the [Van der Waals throttling model](van-der-waals-throttling-model.md) illustrates.

**Table of contents**

- [Joule-Thomson inversion curve](joule-thomson-inversion-curve.md)
  - [Joule-Thomson inversion temperature](joule-thomson-inversion-temperature.md)
- [Van der Waals throttling model](van-der-waals-throttling-model.md)
- [Virial criterion for Joule-Thomson cooling](virial-criterion-for-joule-thomson-cooling.md)

## ↑ Ancestors (6)

1. [Enthalpy](enthalpy-split.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Enthalpy](enthalpy-split.md)
- [Free expansion](free-expansion.md)
- [Helium liquefaction](helium-liquefaction.md)
- [Joule-Thomson coefficient](joule-thomson-coefficient.md)
- [Joule-Thomson effect](joule-thomson-effect.md)
- [Joule-Thomson inversion curve](joule-thomson-inversion-curve.md)
- [Joule-Thomson inversion temperature](joule-thomson-inversion-temperature.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/34d/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2/section-c/c13/solution.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004/section-b/b7/a/solution.md)
- [Van der Waals throttling model](van-der-waals-throttling-model.md)
