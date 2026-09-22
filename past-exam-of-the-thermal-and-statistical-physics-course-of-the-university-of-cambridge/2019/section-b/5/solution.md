<h1 id="section-b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

**[Availability](../../../../exergy.md) and total [entropy](../../../../entropy-split.md).** The reservoir changes by $dU_R=-dU$ and $dV_R=-dV$. Its [particle number](../../../../particle-number.md) and the system's [particle number](../../../../particle-number.md) are fixed. The reservoir's [first law of thermodynamics](../../../../first-law-of-thermodynamics-split.md) therefore gives

$$
dS_R=\frac{dU_R+p_RdV_R}{T_R}
=-\frac{dU+p_RdV}{T_R}.
$$

Add the system's [entropy](../../../../entropy-split.md) change. Because $T_R,p_R$ are constant,

$$
dS_{\mathrm{tot}}=dS-\frac{dU+p_RdV}{T_R}
=-\frac1{T_R}d(U+p_RV-T_RS).
$$

Thus define the [availability](../../../../exergy.md)

$$
\boxed{A=U+p_RV-T_RS,\qquad\Delta S_{\mathrm{tot}}=-\frac{\Delta A}{T_R}.}
$$

An additive constant in $A$ is immaterial; its value above the equilibrium reference is the [exergy](../../../../exergy.md). The [Second law of thermodynamics](../../../../second-law-of-thermodynamics-split.md) gives $\Delta S_{\mathrm{tot}}\geq0$, hence $\Delta A\leq0$. A stable equilibrium maximizes total [entropy](../../../../entropy-split.md) over the allowed variations and therefore minimizes $A$. The environmental $T_R,p_R$ enter this definition even when the system has not yet reached their values. Because both thermal and mechanical exchanges are allowed, equilibrium here includes mechanical balance; equality of temperatures alone does not ensure the minimum.

**[Probability](../../../../probability.md) and curvature.** For a fixed value of a macroscopic coordinate $x$, let $S(x)$ count the compatible system [microstates](../../../../microstate.md). The product of the system and reservoir multiplicities is

$$
\mathcal W(x)\propto
\exp\left[\frac{S(x)}{k_B}-\frac{U(x)+p_RV(x)}{k_BT_R}\right]
=\exp\left[-\frac{A(x)}{k_BT_R}\right].
$$

All factors independent of $x$ enter a normalization constant, giving

$$
\boxed{P(x)=\aleph e^{-A(x)/(k_BT_R)},\qquad
\aleph^{-1}=\int e^{-A(x)/(k_BT_R)}dx.}
$$

Here $A(x)$ is the constrained or effective [availability](../../../../exergy.md) for this coordinate, including the multiplicity of any eliminated variables. A nonuniform coordinate [measure](../../../../measure-split.md) must likewise be retained or incorporated in that effective [availability](../../../../exergy.md).

At a stable interior minimum, $A'(x_0)=0$ and $A''(x_0)>0$. Its [Taylor expansion](../../../../taylor-expansion.md) gives

$$
A(x)=A(x_0)+\frac12A''(x_0)(x-x_0)^2+\cdots.
$$

Keeping the quadratic term yields a [normal distribution](../../../../normal-distribution.md),

$$
P(x)\simeq\sqrt{\frac{A''(x_0)}{2\pi k_BT_R}}
\exp\left[-\frac{A''(x_0)(x-x_0)^2}{2k_BT_R}\right],
\qquad
\boxed{\left\langle(x-x_0)^2\right\rangle\simeq\frac{k_BT_R}{A''(x_0)}.}
$$

This is [availability curvature and equilibrium fluctuations](../../../../availability-curvature-and-equilibrium-fluctuations.md). The quoted fluctuation formula holds at quadratic order in the [Gaussian fluctuation approximation](../../../../gaussian-fluctuation-approximation.md); it is not an exact identity for an arbitrary nonlinear $A(x)$. Higher terms can shift the mean away from its most probable value $x_0$.

**Bubble equilibrium.** Keep the number of air [molecules](../../../../molecule-split.md) fixed and include the [surface energy](../../../../surface-energy.md) in the system's total [internal energy](../../../../internal-energy-split.md). For constant [surface tension](../../../../surface-tension-split.md) $\Gamma$, this contribution is $\Gamma\Omega=\Gamma\alpha V^{2/3}$, with no surface [entropy](../../../../entropy-split.md) under the stated approximation. Its differential is

$$
dU=T\,dS-p_{\mathrm{air}}\,dV+\Gamma\,d\Omega.
$$

Hence

$$
dA=(T-T_R)dS+
\left[p_R-p_{\mathrm{air}}+\frac23\Gamma\alpha V^{-1/3}\right]dV.
$$

Independent thermal and [volume](../../../../volume-thermodynamics.md) variations give $T=T_R$ and

$$
\boxed{p_{\mathrm{air}}-p_R=\frac23\Gamma\alpha V_0^{-1/3},\qquad
V_0=\left[\frac{2\Gamma\alpha}{3(p_{\mathrm{air}}-p_R)}\right]^3.}
$$

The air [pressure](../../../../pressure-split.md) is evaluated at $V_0$; since the bubble is closed it generally depends on [volume](../../../../volume-thermodynamics.md), so this equation is implicit until an air [equation of state](../../../../equation-of-state.md) is supplied. For a [sphere](../../../../sphere.md), $\alpha=(36\pi)^{1/3}$, $\Omega=4\pi R^2$, and the [pressure](../../../../pressure-split.md) jump becomes $2\Gamma/R$, the [Young–Laplace equation](../../../../young-laplace-equation.md) for a single gas–liquid interface. There is no second surface as in a thin soap film.

**Isothermal [volume](../../../../volume-thermodynamics.md) fluctuations.** With the air maintained at $T_R$, eliminate its [entropy](../../../../entropy-split.md) in favor of its [Helmholtz free energy](../../../../helmholtz-free-energy.md):

$$
A_T(V)=F_{\mathrm{air}}(T_R,V,N)+p_RV+\Gamma\alpha V^{2/3}.
$$

The identity $(\partial F_{\mathrm{air}}/\partial V)_{T,N}=-p_{\mathrm{air}}$ gives

$$
A_T''(V_0)
=-\left(\frac{\partial p_{\mathrm{air}}}{\partial V}\right)_{T_R,N,V_0}
-\frac29\Gamma\alpha V_0^{-4/3}
=\frac1{V_0}\left[\kappa_T^{-1}-\frac29\Gamma\alpha V_0^{-1/3}\right].
$$

Using the curvature result,

$$
\boxed{\left\langle\Delta V^2\right\rangle\simeq
\frac{k_BT_RV_0}{\kappa_T^{-1}-\frac29\Gamma\alpha V_0^{-1/3}}.}
$$

These are the [volume fluctuations of a closed gas bubble](../../../../volume-fluctuations-of-a-closed-gas-bubble.md). Stability requires the denominator to be positive. The negative surface contribution reflects the concavity of $V^{2/3}$; gas compression supplies the positive restoring curvature. For ideal air, $\kappa_T^{-1}=p_{\mathrm{air}}$, and [mechanical equilibrium](../../../../mechanical-equilibrium.md) reduces the denominator to

$$
\boxed{D=p_R+\frac49\Gamma\alpha V_0^{-1/3}>0.}
$$

The units are consistent: $D$ is [pressure](../../../../pressure-split.md), so $k_BT_RV_0/D$ has units $\mathrm{m^6}$, the units of a [volume](../../../../volume-thermodynamics.md) [variance](../../../../variance-split.md). Holding $p_{\mathrm{air}}$ externally fixed while varying $V$ would remove the gas-compression term and change this stability problem; that is not the fixed-particle-number situation here.

**Numerical size of the fluctuations.** The [volume](../../../../volume-thermodynamics.md) conversion is important:

$$
V_0=10^{-3}\,\mathrm{mm^3}=10^{-12}\,\mathrm{m^3},\qquad
V_0^{1/3}=10^{-4}\,\mathrm m,\qquad T_R=298.15\,\mathrm K.
$$

Use the specified $\alpha=4.84$, $\Gamma=0.072\,\mathrm{N\,m^{-1}}$ and $p_R=10^5\,\mathrm{Pa}$. Then

$$
p_{\mathrm{air}}-p_R
=\frac23(0.072)(4.84)(10^4)\,\mathrm{Pa}
=2323.2\,\mathrm{Pa},
$$



$$
D=10^5+\frac49(0.072)(4.84)(10^4)
=101548.8\,\mathrm{Pa}.
$$

With the [Boltzmann constant](../../../../boltzmann-constant.md) $k_B=1.380649\times10^{-23}\,\mathrm{J\,K^{-1}}$,

$$
k_BT_R=4.1164\times10^{-21}\,\mathrm J,
\qquad
\left\langle\Delta V^2\right\rangle\simeq4.05\times10^{-38}\,\mathrm{m^6}.
$$

Thus the fractional [root mean square](../../../../root-mean-square.md) fluctuation and fractional [variance](../../../../variance-split.md) are respectively

$$
\boxed{\frac{\sqrt{\langle\Delta V^2\rangle}}{V_0}\simeq2.01\times10^{-7},
\qquad\frac{\langle\Delta V^2\rangle}{V_0^2}\simeq4.05\times10^{-14}.}
$$

The absolute [root mean square](../../../../root-mean-square.md) fluctuation is $2.01\times10^{-19}\,\mathrm{m^3}$. The very small fractional value supports the local [Gaussian fluctuation approximation](../../../../gaussian-fluctuation-approximation.md). This estimate neglects exchange of dissolved air, variations of [surface tension](../../../../surface-tension-split.md), shape fluctuations and [temperature](../../../../temperature-split.md) fluctuations, consistently with the prescribed fixed-number, isothermal bubble model.

## ↑ Ancestors (13)

1. [5](../5.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
