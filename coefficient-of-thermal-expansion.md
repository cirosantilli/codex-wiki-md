# Coefficient of thermal expansion

↑ **Parent:** [Thermal expansion](thermal-expansion.md)

The volumetric coefficient of [thermal expansion](thermal-expansion.md) is the fractional [volume](volume-thermodynamics.md) increase per [temperature](temperature.md) increase at fixed [pressure](pressure.md) and composition:

$$
\alpha=\frac1V\left(\frac{\partial V}{\partial T}\right)_{P,N}
=-\frac1\rho\left(\frac{\partial\rho}{\partial T}\right)_{P,N},\qquad
\rho=\frac mV.
$$

The [mass density](density.md) form requires fixed [mass](mass.md) $m$. Its units are $\mathrm{K^{-1}}$; $\alpha_T$ is another notation for this coefficient. For small [temperature](temperature.md) changes $\theta$ at fixed [pressure](pressure.md),

$$
V(T_0+\theta)\simeq V(T_0)(1+\alpha(T_0)\theta),\qquad
\rho(T_0+\theta)\simeq\rho(T_0)(1-\alpha(T_0)\theta).
$$

For a finite change in a single [thermodynamic phase](thermodynamic-phase.md), integrate the possibly varying coefficient: $\ln(V_2/V_1)=\int_{T_1}^{T_2}\alpha(T,P,N)\,dT$. A constant-coefficient approximation gives an exponential, while the displayed linear formula additionally requires $|\alpha\theta|\ll1$.

For an [ideal gas](ideal-gas.md) at fixed particle number,

$$
\alpha=\frac1T,\qquad
\alpha(300\,\mathrm K)=\frac1{300}\,\mathrm{K^{-1}}\simeq3.333\times10^{-3}\,\mathrm{K^{-1}}.
$$

Integrating $1/T$ recovers the exact fixed-[pressure](pressure.md) [thermal expansion](thermal-expansion.md) ratio $V_2/V_1=T_2/T_1$. Combining expansion with [isothermal compressibility](isothermal-compressibility.md) gives the local response of any smooth [simple compressible system](simple-compressible-system.md) of fixed composition,

$$
\frac{dV}{V}=\alpha\,dT-\kappa_T\,dP,\qquad
\left(\frac{\partial P}{\partial T}\right)_{V,N}=\frac\alpha{\kappa_T}.
$$

The ratio has units $\mathrm{Pa\,K^{-1}}$. For the one-[mole](mole-unit.md) [ideal gas](ideal-gas.md) state in [isothermal compressibility](isothermal-compressibility.md), it is $P_0/T_0=333.33\,\mathrm{Pa\,K^{-1}}$: a $1\,\mathrm K$ increase at fixed [volume](volume-thermodynamics.md) raises the [pressure](pressure.md) by about $333.33\,\mathrm{Pa}$. [Maxwell relations](maxwell-relations.md) identify this same ratio as the [entropy](entropy.md) slope with respect to [volume](volume-thermodynamics.md) and give $C_P-C_V=TV\alpha^2/\kappa_T$.

Under the [Boussinesq approximation](boussinesq-approximation.md), the small fractional [mass density](density.md) change produces [buoyancy](buoyancy.md) while [mass density](density.md) is otherwise treated as constant. A positive [temperature](temperature.md) excess $\theta$ gives [reduced gravity](reduced-gravity-split.md) $g'=g\alpha_T\theta$ in the convention used in [natural ventilation](natural-ventilation.md). The coefficient therefore converts a [heat](heat.md) budget into a buoyancy budget. The same measurable expansion response supplies [entropy](entropy.md) changes and [heat capacity](heat-capacity.md) differences through [Maxwell relations](maxwell-relations.md), connecting fluid motion to equilibrium [thermodynamics](thermodynamics-split.md).

## ↑ Ancestors (6)

1. [Thermal expansion](thermal-expansion.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Compressibility](compressibility.md)
- [Dulong-Petit law](dulong-petit-law.md)
- [Linear thermal expansion coefficient](linear-thermal-expansion-coefficient.md)
- [Maxwell relations](maxwell-relations.md)
- [Mayer's relation](mayer-s-relation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-77/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-69/5/solution.md)
- [Thermal expansion](thermal-expansion.md)
