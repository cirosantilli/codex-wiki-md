<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $V_b$ be the northward speed in the [western boundary current](../../../../western-boundary-current.md), whose zonal width $\delta$ is much less than its meridional scale. Its dominant [relative vorticity](../../../../relative-vorticity.md) is $\xi\simeq v_x\sim V_b/\delta$. Neglecting local [wind stress curl](../../../../wind-stress-curl.md) and relative-[vorticity](../../../../vorticity-split.md) advection in the narrow return region, the linear stationary [vorticity equation](../../../../vorticity-equation.md) becomes

$$
\beta v\simeq-r\xi\simeq-rv_x.
$$

Consequently

$$
\boxed{\delta\sim\frac r\beta,\qquad v(x,y)\propto e^{-x/\delta}.}
$$

This decay into the interior from the western wall explains why the [Stommel boundary layer](../../../../stommel-boundary-layer.md) lies on the west. The sign also matters: a northward return has $v_x<0$, so its negative [relative vorticity](../../../../relative-vorticity.md) supplies a positive drag contribution $-r\xi$ to balance $\beta v$. Here $r$ has units $\mathrm{s^{-1}}$; no extra factor of $f_0$ belongs in $r/\beta$ with the paper's definition of [linear drag](../../../../linear-drag.md).

For example, at fixed $y$ the leading correction to the interior [ocean transport streamfunction](../../../../ocean-transport-streamfunction.md) is

$$
\Psi_B=LV(y)e^{-x/\delta},\qquad
Hv_B=\partial_x\Psi_B=-\frac{LV(y)}\delta e^{-x/\delta}.
$$

It cancels the western value of $\Psi_I$ and carries $\int_0^\infty Hv_B\,dx=-LV=-T$. Exponentially small eastern-wall corrections and the turning regions near the northern and southern walls do not affect the leading width estimate.

Using one year $=3.156\times10^7\ \mathrm s$, the representative $\beta$ of 2(b), and $H=10^3\ \mathrm m$ gives

$$
r=3.17\times10^{-8}\ \mathrm{s^{-1}},\qquad
\boxed{\delta\simeq1.58\times10^3\ \mathrm m=1.6\ \mathrm{km}.}
$$

To return the $25\ \mathrm{Sv}$ interior [volume flux](../../../../volumetric-flow-rate.md), [conservation of mass](../../../../mass-conservation.md) requires

$$
\boxed{V_b\sim\frac{|T|}{H\delta}
\simeq15.8\ \mathrm{m\,s^{-1}}.}
$$

For the exponential profile this is the boundary speed associated with its effective transport width $\delta$. It is much narrower and faster than the familiar large-scale [western boundary currents](../../../../western-boundary-current.md), whose energetic cores span tens of kilometres and have speeds of order $1\ \mathrm{m\,s^{-1}}$. The simplified constant-depth [linear drag](../../../../linear-drag.md) model with a one-year decay time therefore does not give a realistic quantitative boundary structure. [Lateral viscosity](../../../../lateral-viscosity.md), [eddies](../../../../eddy.md), [stratification](../../../../density-stratification.md) and inertia can all affect a real current.

The corresponding [relative vorticity](../../../../relative-vorticity.md) scale is

$$
\boxed{|\xi|\sim\frac{V_b}\delta\simeq9.96\times10^{-3}\ \mathrm{s^{-1}},\qquad
\frac{|\xi|}{|f_0|}\sim100\quad\text{for }|f_0|\sim10^{-4}\ \mathrm{s^{-1}}.}
$$

Thus [relative vorticity](../../../../relative-vorticity.md) cannot be discarded relative to [planetary vorticity](../../../../planetary-vorticity.md) in this predicted return. Even a more realistic $1\ \mathrm{m\,s^{-1}}$ across $50\ \mathrm{km}$ gives $|\xi|\sim2\times10^{-5}\ \mathrm{s^{-1}}$, an appreciable fraction of $|f_0|$.

Magnitude alone does not prove that its material [advection](../../../../advection.md) is large: a perfectly parallel current $v=v(x)$, $u=0$ has $\mathbf u\cdot\nabla\xi=0$ exactly. For a gyre return varying over meridional scale $B$, however, [incompressibility](../../../../incompressible-flow.md) gives $u\sim\delta V_b/B$, and both generic contributions to $\mathbf u\cdot\nabla\xi$ scale as $V_b^2/(B\delta)$. Relative to $\beta V_b$, this is

$$
\frac{|\mathbf u\cdot\nabla\xi|}{\beta V_b}
\sim\frac{V_b}{\beta B\delta}
\simeq1.6\times10^2\qquad(B=\pi\times10^6\ \mathrm m).
$$

Absent special cancellations, the assumed neglect of relative-[vorticity](../../../../vorticity-split.md) advection is therefore not self-consistent for these parameters. Its natural inertial width is instead $\delta_I\sim\sqrt{V_I/\beta}$, where $V_I=|T|/(HL)\simeq5\times10^{-3}\ \mathrm{m\,s^{-1}}$; this gives about $16\ \mathrm{km}$. That comparison diagnoses the missing inertia rather than supplying a complete nonlinear boundary-current solution.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the geophysical fluid dynamics course of the University of Oxford](../../../split.md)
5. [Geophysical fluid dynamics course of the University of Oxford](../../../../geophysical-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
