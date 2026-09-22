<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a stationary, uniformly permeable skeleton, [Darcy law](../../../../../darcy-law.md) gives $\mathbf u=-(\Pi/\mu)\nabla p$. Constant-density [conservation of mass](../../../../../mass-conservation.md) gives $\nabla\cdot\mathbf u=0$, hence **the [pressure](../../../../../pressure.md) is harmonic**:

$$
\boxed{\nabla^2p=0.}
$$

With uniform [gravitational acceleration](../../../../../gravitational-acceleration.md), the same argument applies to [pressure](../../../../../pressure.md) after subtracting its hydrostatic part. The spherical calculation below neglects body-force variation and uses the excess [pressure](../../../../../pressure.md) relative to the far field.

Set $\epsilon=1-\rho_s/\rho>0$ and $\beta=\phi\epsilon$. When a shell freezes, its pore mass decreases at rate $4\pi a^2\phi(\rho-\rho_s)\dot a$; the difference must leave as liquid. Since [Darcy velocity](../../../../../darcy-velocity.md) is volume discharge per total area, not pore-fluid speed, the interfacial and radial balances give

$$
\rho u(a)=\phi(\rho-\rho_s)\dot a,\qquad\boxed{u(r,t)=\beta\dot a\frac{a^2}{r^2}\quad(r\geq a).}
$$

The positive sign means outward expulsion by the expansion on freezing. Integrating [Darcy law](../../../../../darcy-law.md) with $p(\infty)=0$ gives

$$
\boxed{p(r,t)=\frac{\mu\beta a^2\dot a}{\Pi r},\qquad p_i=p(a,t)=\frac{\mu\beta a\dot a}{\Pi}.}
$$

There is no liquid [Darcy velocity](../../../../../darcy-velocity.md) in the ice-filled region.

To state a closed [Stefan problem](../../../../../stefan-problem.md), let $k_-,k_+$ be the effective [thermal conductivities](../../../../../thermal-conductivity.md) of the frozen and unfrozen composites and $C_-,C_+$ their volumetric [heat capacities](../../../../../heat-capacity.md). If the matrix [mass density](../../../../../density.md) is $\rho_m$, the common specific heat gives $C_-=c_p[(1-\phi)\rho_m+\phi\rho_s]$ and $C_+=c_p[(1-\phi)\rho_m+\phi\rho]$. These material coefficients are not numerically specified. With $\mathcal L=\phi\rho_sL$, the thermal equations are

$$
C_-\partial_tT_-=k_-\frac1{r^2}\partial_r(r^2\partial_rT_-),\quad 0<r<a,
$$



$$
C_+\partial_tT_++\rho c_pu\partial_rT_+=k_+\frac1{r^2}\partial_r(r^2\partial_rT_+),\quad r>a.
$$

The exterior equation retains advected sensible heat. A more detailed mechanical-energy model adds the [Darcy dissipation](../../../../../darcy-dissipation.md) source $\mu u^2/\Pi$; its smallness at leading order is checked below. At the origin require $\partial_rT_-(0)=0$, and at infinity require $T_+\to T_\infty$, $p\to0$. At the [phase boundary](../../../../../phase-boundary.md) impose [temperature](../../../../../temperature.md) continuity, phase equilibrium and the [Stefan condition](../../../../../stefan-condition.md):

$$
T_-(a)=T_+(a)=T_i=T_m-\gamma p_i,\qquad \gamma=\frac{T_m\epsilon}{\rho_sL},
$$



$$
\mathcal L\dot a=k_-\partial_rT_-(a^-)-k_+\partial_rT_+(a^+).
$$

These equations, the radial liquid-mass balance and [Darcy law](../../../../../darcy-law.md), together with an initial radius and compatible initial [temperature](../../../../../temperature.md) fields, specify the moving-boundary model. No curvature correction is imposed. A vanishing initial seed corresponds to the leading growth law below with $a(0)=0$.

Write $\Delta=T_m-T_\infty$ and $S=L/(c_p\Delta)$, the [latent-to-sensible heat ratio](../../../../../latent-to-sensible-heat-ratio.md). A conductive interfacial balance gives $a\dot a\lesssim k_+\Delta/\mathcal L$. On length scale $a$, the ratio of thermal diffusion time to growth time is consequently bounded by

$$
\frac{t_{\rm diff}}{t_{\rm grow}}\lesssim\frac{C_\pm\Delta}{\phi\rho_sL}.
$$

It is small for $S\gg1$ with fixed [porosity](../../../../../porosity.md) and comparable constituent densities and thermal properties. Very small [porosity](../../../../../porosity.md) requires the sharper condition $C_\pm\Delta/(\phi\rho_sL)\ll1$; the bare heat-capacity ratio alone should not be used uniformly as $\phi\to0$. The advective-to-conductive ratio is

$$
\frac{\rho c_pu(a)a}{k_+}=\frac{\rho c_p\beta a\dot a}{k_+}\lesssim\frac{\rho\epsilon}{\rho_sS}\ll1.
$$

Even if mechanical heating is retained, its size relative to latent-heat release is $p_i\beta/\mathcal L=(T_m-T_i)/T_m\leq\Delta/T_m$. For fixed water properties this is also small as $S\to\infty$, consistently with the linearized [Clausius-Clapeyron relation](../../../../../clausius-clapeyron-relation.md). Thus unsteadiness, thermal [advection](../../../../../advection.md) and mechanical heating are higher-order effects. **The local leading [temperature](../../../../../temperature.md) fields satisfy Laplace's equation.** The approximation describes radii of order $a$; the distant transient diffusion tail supplies the far-field matching and need not be globally steady.

Regularity at zero and the interface/far-field values give

$$
\boxed{T_-(r)=T_i,\qquad T_+(r)=T_\infty+(T_i-T_\infty)\frac ar.}
$$

The [Stefan condition](../../../../../stefan-condition.md) becomes $\mathcal L a\dot a=k_+(T_i-T_\infty)$. Introduce the dimensionless [pressure](../../../../../pressure.md)-feedback factor

$$
\Lambda=\frac{k_+\gamma\mu\beta}{\Pi\mathcal L}=\frac{k_+\mu T_m\epsilon^2}{\Pi\rho_s^2L^2}.
$$

Combining this heat balance with [pressure](../../../../../pressure.md)-dependent phase equilibrium yields **the growth and interface values**:

$$
\boxed{a\dot a=\frac{k_+\Delta}{\mathcal L(1+\Lambda)},\qquad a(t)^2=a_0^2+\frac{2k_+\Delta}{\mathcal L(1+\Lambda)}(t-t_0),}
$$



$$
\boxed{T_i=T_\infty+\frac{\Delta}{1+\Lambda},\qquad p_i=\frac{\Delta}{\gamma}\frac{\Lambda}{1+\Lambda}.}
$$

This is [pressure-limited spherical freezing in a porous medium](../../../../../pressure-limited-spherical-freezing-in-a-porous-medium.md). The interface values are constant during this leading solution, although $p(r,t)$ changes at a fixed exterior radius.

As [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md) decreases, $\Lambda$ increases: the interface [pressure](../../../../../pressure.md) rises toward the finite value $\Delta/\gamma$, while the interface [temperature](../../../../../temperature.md) falls toward $T_\infty$. Hydraulic resistance suppresses freezing through [pressure](../../../../../pressure.md)-induced [freezing-point depression](../../../../../freezing-point-depression.md). In the limit $\Pi\to0$, $a\dot a\sim\Pi\Delta/(\gamma\mu\beta)$; **a zero-seed radius grows as $\sqrt{\Pi t}$ and tends to zero at fixed time**. A finite seed instead hardly changes. At exactly zero permeability an incompressible rigid model cannot expel the expansion volume, so sustained growth stops; deformation or compressibility would require a different model.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
