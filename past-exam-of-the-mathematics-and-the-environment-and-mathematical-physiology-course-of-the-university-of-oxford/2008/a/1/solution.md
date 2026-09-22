<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The left side is atmospheric heat storage per unit surface area. Incoming solar flux $Q$ is averaged over the spherical surface by the factor $1/4$; [albedo](../../../../albedo.md) $a$ reflects a fraction of it. The outgoing term is a reduced Stefan-Boltzmann flux, with effective emissivity $\gamma$ representing atmospheric greenhouse trapping. [Ice-albedo feedback](../../../../ice-albedo-feedback.md) usually makes $a$ decrease as [temperature](../../../../temperature-split.md) rises through an [ice](../../../../ice.md)-melting range; greater carbon-dioxide [pressure](../../../../pressure-split.md) increases infrared opacity and therefore decreases this effective $\gamma$. The simple estimates below hold [albedo](../../../../albedo.md) fixed.

[Radiative equilibrium](../../../../radiative-equilibrium.md) gives

$$
\boxed{\gamma_0=\frac{(1-a)Q}{4\sigma T_0^4}\simeq0.5978.}
$$

Differentiating $\gamma T^4=\text{constant}$ gives $\Delta\gamma\simeq-4\gamma_0\Delta T/T_0\simeq-0.02474$. A doubling from $36$ Pa changes [pressure](../../../../pressure-split.md) by $36$ Pa, hence

$$
\boxed{\gamma_1\simeq\frac{4\gamma_0\cdot3}{290\cdot36}=6.87\times10^{-4}\ {\rm Pa}^{-1}.}
$$

Reference [weathering](../../../../weathering.md) balance requires $A_LW_0=v_0$, so $\boxed{W_0=2.0\times10^{-3}\ {\rm kg\,m^{-2}\,yr^{-1}}}$.

For the requested approximate system, take $(T_0,p_0)$ as the reference radiative/[weathering](../../../../weathering.md) [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md), set $\theta=(T-T_0)/\Delta T_c$, $P=p/p_0$, and $\hat t=t/t_{\rm CO_2}$, where

$$
\boxed{t_{\rm CO_2}=\frac{M_{\rm CO_2}Ap_0}{M_agv_0},\quad
 t_T=\frac{\rho_ac_pd}{4\sigma\gamma_0T_0^3},\quad
\epsilon=\frac{t_T}{t_{\rm CO_2}},\quad
\Gamma=\frac{\gamma_1p_0T_0}{4\gamma_0\Delta T_c}.}
$$

Linearize the radiative loss, retaining terms linear in $T-T_0$ and $p-p_0$. Its two terms are $4\sigma\gamma_0T_0^3(T-T_0)$ and $-\sigma\gamma_1T_0^4(p-p_0)$. The carbon balance scales exactly with $v=v_{\rm CO_2}/v_0$. Therefore

$$
\boxed{\epsilon\theta_{\hat t}=-\theta+\Gamma(P-1),\qquad P_{\hat t}=v-P^\mu e^\theta.}
$$

Numerically $\boxed{t_{\rm CO_2}\simeq7.41\times10^3\ {\rm yr},\quad t_T\simeq0.0958\ {\rm yr},\quad\epsilon\simeq1.29\times10^{-5},\quad\Gamma\simeq0.1795}$. The time conversion uses seconds for the radiative constants and years for the supplied carbon production.

Because $\epsilon\ll1$, [temperature](../../../../temperature-split.md) rapidly approaches $\theta=\Gamma(P-1)$, while carbon changes slowly. A sustained $v\simeq40$ has [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) determined by

$$
\mu\log P_*+\Gamma(P_*-1)=\log40.
$$

Its left side is [strictly increasing](../../../../strictly-increasing-function.md) on positive [pressure](../../../../pressure-split.md), giving $\boxed{P_*\simeq16.83,\quad\Delta T_{\rm eventual}=\Delta T_c\Gamma(P_*-1)\simeq36.9\ {\rm K}}$ within this extrapolated toy model. Counting volcanic production as well gives $v=41$ and $37.2$ K instead. An inventory estimate for the rise is $t_{\rm CO_2}(P_*-1)/(v-1)\simeq3.0\times10^3$ years. [Linearization](../../../../linearization.md) near the final [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) gives the [e-folding time](../../../../exponential-relaxation-time.md)

$$
\boxed{t_{\rm relax}=\frac{t_{\rm CO_2}}{v(\Gamma+\mu/P_*)}\simeq9.4\times10^2\ {\rm yr}.}
$$

Thus the carbon/[weathering](../../../../weathering.md) response is millennial, despite the short [thermal adjustment](../../../../radiative-relaxation-time-in-a-planetary-atmosphere.md) time.

There are two numerical-reference inconsistencies in the printed setup. The requested expansion treats $(T_0,p_0)$ as its reference [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) although earlier labels pair $T_0$ with present-day $36$ Pa rather than $p_0=28$ Pa. Also, the calibrated $\Gamma=0.1795$ gives $13^{0.3}e^{13\Gamma}\simeq22.3$, not the stated hint. That hint instead corresponds to $\Gamma\simeq3/13$, obtained by calibrating a doubling of $28$ Pa. Such a convention gives a [pressure](../../../../pressure-split.md) around $13$–$14$ and a similar rough warming of several tens of kelvin. The displayed results above consistently use the stated $36$ Pa doubling calibration and explicitly declared reference-model approximation. A large extrapolation of a linearized radiative law is a property of this exercise, not a quantitative climate projection.

This is a [weathering feedback with fast thermal adjustment](../../../../weathering-feedback-with-fast-thermal-adjustment.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
