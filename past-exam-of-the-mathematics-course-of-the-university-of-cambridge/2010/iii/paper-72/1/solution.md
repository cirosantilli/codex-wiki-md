<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\epsilon=1-\rho_s/\rho>0$ and $\Delta v=1/\rho_s-1/\rho=\epsilon/\rho_s$. When the [ice](../../../../../ice.md) sphere grows by volume $4\pi a^2\dot a\,dt$, it consumes liquid volume $(\rho_s/\rho)4\pi a^2\dot a\,dt$. The difference is expelled from the fixed cavity. Thus [mass conservation](../../../../../mass-conservation.md) fixes the outward [Darcy flux](../../../../../darcy-velocity.md) in the surrounding [porous medium](../../../../../porous-medium.md):

$$
4\pi r^2u_r=4\pi\epsilon a^2\dot a,\qquad u_r=\frac{\epsilon a^2\dot a}{r^2}\quad(r\ge R).
$$

The [Darcy law](../../../../../darcy-law.md) $u_r=-(\Pi/\mu)\partial_rp$ and $p(\infty)=p_m$ imply

$$
p(r)-p_m=\frac{\mu\epsilon a^2\dot a}{\Pi r}.
$$

Matching at the cavity wall, whose internal [pressure](../../../../../pressure.md) is uniform, gives

$$
\boxed{p-p_m=\frac\mu\Pi\left(1-\frac{\rho_s}{\rho}\right)\frac{a^2\dot a}{R}.}
$$

The solid and liquid pressures are equal when the [Gibbs--Thomson relation](../../../../../gibbs-thomson-relation.md) is neglected; nevertheless the coexistence [temperature](../../../../../temperature.md) changes with their common pressure because their specific volumes differ. Along coexistence, equality of [chemical potentials](../../../../../chemical-potential.md) gives

$$
-(s_l-s_s)dT+(1/\rho-1/\rho_s)dp=0,\qquad s_l-s_s=L/T_m.
$$

Hence the [common-pressure melting-point slope](../../../../../common-pressure-melting-point-slope.md) is $dT_m/dp=-T_m\Delta v/L$. To first order in the pressure change,

$$
T_i=T_m-\gamma_p(p-p_m),\qquad \gamma_p=\frac{T_m\Delta v}{L}>0.
$$

The $T_m$ multiplying this coefficient is absolute [temperature](../../../../../temperature.md), approximately $273.15\,\mathrm K$ for water; a temperature difference may equally be measured in kelvin or degrees Celsius. Substituting the numerical value $0$ from the Celsius scale into a thermodynamic denominator would be incorrect.

In the quasi-stationary [thermal conduction](../../../../../thermal-conduction.md) approximation, neglect advective heat transport and use the stated effective conductivity $k$ outside the sphere. The radial [Laplace equation](../../../../../laplace-equation.md) gives the bounded solid [temperature](../../../../../temperature.md) and the liquid/porous-region [temperature](../../../../../temperature.md):

$$
\boxed{T_s(r)=T_i\quad(0\le r<a),\qquad T_l(r)=T_\infty+(T_i-T_\infty)\frac ar\quad(r>a).}
$$

This treats the exterior as a uniform conducting medium, as required by the printed reduction; distinct cavity and porous-medium conductivities would give an additional thermal resistance. There is no solid-side [heat flux](../../../../../heat-flux-density.md) in the bounded quasi-stationary solution. The [Stefan condition](../../../../../stefan-condition.md) therefore becomes

$$
\rho_sL\dot a=-k\partial_rT_l(a)=\frac{k(T_i-T_\infty)}a.
$$

Eliminate $T_i$ and $p$ to obtain

$$
\left(a+\frac{a^2}{KR}\right)\dot a=\frac{k\Delta T}{\rho_sL},\qquad
\Delta T=T_m-T_\infty,\qquad
K=\frac{L^2\Pi}{(\Delta v)^2kT_m\mu}.
$$

For $x=a/R$, $t=t_0\tau$ and $t_0=R^2\rho_sL/(k\Delta T)$, this is

$$
\boxed{\left(x+\frac{x^2}{K}\right)\frac{dx}{d\tau}=1.}
$$

The [pressure](../../../../../pressure.md) follows either from the [Darcy flux](../../../../../darcy-velocity.md) or the [Stefan condition](../../../../../stefan-condition.md):

$$
\boxed{p-p_m=p^*\frac{x}{x+K},\qquad
p^*=\frac{\Delta T}{\gamma_p}=\rho_sL\frac{\Delta T}{T_m}\left(1-\frac{\rho_s}{\rho}\right)^{-1}.}
$$

In particular $T_i-T_\infty=\Delta T K/(x+K)$: rising pressure progressively reduces the available undercooling. This is [spherical freezing inside a porous cavity](../../../../../spherical-freezing-inside-a-porous-cavity.md), whose fixed hydraulic outlet radius $R$ distinguishes it from freezing directly through a porous matrix.

For the idealized zero-radius start, integration gives

$$
\boxed{\tau=\frac{x^2}{2}+\frac{x^3}{3K},\qquad 0\le x\le1.}
$$

A finite seed replaces the right side by its difference from the initial value. The reduction ends when the sphere fills the cavity.

For $K\gg1$, hydraulic drainage is easy and the pressure feedback is small throughout the cavity. The leading expressions are

$$
\boxed{p(x)=p_m+\frac{p^*}{K}x+O(K^{-2}p^*),\qquad
x(t)\simeq\sqrt{\frac{2t}{t_0}},\qquad
a(t)\simeq\sqrt{\frac{2k\Delta T}{\rho_sL}t}.}
$$

This is ordinary conduction-controlled spherical [solidification](../../../../../freezing.md), with a completion time asymptotic to $t_0/2$.

For $K\ll1$, distinguish the initial crossover from the pressure-dominated regime. At $x\ll K$, equivalently $\tau\ll K^2$, the same square-root growth applies and $p-p_m\simeq p^*x/K$. At $K\ll x\le1$, equivalently $K^2\ll\tau\lesssim1/K$,

$$
\boxed{x(t)\simeq\left(\frac{3Kt}{t_0}\right)^{1/3},\qquad
p(x)=p_m+p^*\left[1-\frac Kx+O\!\left(\frac{K^2}{x^2}\right)\right].}
$$

The interface approaches $T_\infty$, the pressure approaches the finite coexistence value $p_m+p^*$, and growth becomes hydraulically limited. The leading completion time is $t_0/(3K)$. The cube-root approximation is not valid at the instant of nucleation, where the initial square-root regime must be retained.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
