<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose the positive $x$ direction along the background flow, so $U>0$; reverse $x$ if necessary. Let $z$ measure depth below the impermeable roof, and set $\Delta\rho=\rho_w-\rho_c>0$. The deep ambient [water](../../../../../water.md) has $p_w=p_0(x)+\rho_wgz$. Continuity of [pressure](../../../../../pressure.md) at $z=h$ and [hydrostatic pressure](../../../../../hydrostatic-pressure.md) inside the buoyant [CO2](../../../../../carbon-dioxide.md) give

$$
p_c=p_0(x)+\Delta\rho gh+\rho_cgz,\qquad
u_D=-\frac k\mu\partial_xp_c=U-K_bh_x,\qquad K_b=\frac{k\Delta\rho g}{\mu}.
$$

Here $k$ is [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md) and $\mu$ is [dynamic viscosity](../../../../../dynamic-viscosity.md). Since $h/H\ll1$, the ambient return-flow correction to the imposed [pressure gradient](../../../../../pressure-gradient.md) is higher order. The small aspect ratio supplies the [hydrostatic pressure](../../../../../hydrostatic-pressure.md) approximation; capillary trapping, dissolution, compressibility and dispersion are omitted in this sharp-interface model.

The depth-integrated [Darcy flux](../../../../../darcy-velocity.md) is $q=Uh-K_bhh_x$. The actual stored fluid volume is $\phi h$ per unit horizontal area, where $\phi$ is the aquifer [porosity](../../../../../porosity.md). Thus the [porous gravity current with background flow](../../../../../porous-gravity-current-with-background-flow.md) satisfies

$$
\boxed{\phi h_t+\partial_x(Uh-K_bhh_x)=Q\delta_0(x),\qquad
h_t+u h_x=a(hh_x)_x+J\delta_0(x),}
$$

with $u=U/\phi$, $a=K_b/\phi$ and $J=Q/\phi$. Both $Q$ and the later $V$ denote actual injected volume per unit transverse width. Away from injection, the equation is an advected [porous medium equation](../../../../../porous-medium-equation.md). At each finite front impose $h=0$ and vanishing outgoing [volume flux per unit width](../../../../../volume-flux-per-unit-width.md). At the injection point $h$ is continuous and $q(0^+)-q(0^-)=Q$. For an initially empty aquifer, $\phi\int h\,dx=Qt$. **The advective speed is $U/\phi$, not $U$.**

For a [constant-flux porous gravity current](../../../../../constant-flux-porous-gravity-current.md), write characteristic depth $H_c$ and extent $L_c$ temporarily. At early times [volume conservation](../../../../../volume-conservation.md) gives $H_c L_c\sim Jt$; gravity spreading gives $L_c^2/t\sim a H_c$. Hence

$$
\boxed{L_c\sim(aJ)^{1/3}t^{2/3},\qquad H_c\sim(J^2/a)^{1/3}t^{1/3}.}
$$

Background [advection](../../../../../advection.md) becomes comparable when $L_c\sim ut$, so the transition scales are

$$
\boxed{t_c=\frac{aJ}{u^3}=\frac{\phi K_bQ}{U^3},\qquad
\ell_c=ut_c=\frac{K_bQ}{U^2},\qquad h_c=\frac Ju=\frac QU.}
$$

For $t\ll t_c$, the leading [similarity solution](../../../../../similarity-solution.md) is symmetric:

$$
h=(J^2/a)^{1/3}t^{1/3}F(\eta),\qquad
\eta=\frac{x}{(aJ)^{1/3}t^{2/3}}.
$$

For $0<\eta<\eta_N$, its model [ordinary differential equation](../../../../../ordinary-differential-equation.md) and boundary conditions are

$$
\boxed{(FF')'+\frac23\eta F'-\frac13F=0,\qquad
-F(0)F'(0^+)=\frac12,\qquad F(\eta_N)=0.}
$$

Choose the nonnegative finite-front branch, reflect evenly in $x$, and require $FF'\to0$ at the front. The factor $1/2$ divides the injection equally between the two halves. Integration of the [ordinary differential equation](../../../../../ordinary-differential-equation.md) gives $2\int_0^{\eta_N}F\,d\eta=1$; the limiting front slope is $F'(\eta_N^-)=-2\eta_N/3$. This boundary-value problem determines the initially symmetric shape without assuming an unjustified elementary formula. Independent numerical integration gives $\eta_N\simeq1.17619$ in this normalization.

For $t\gg t_c$, upstream storage approaches a finite steady value. With no upstream leakage, $q=0$ for $x<0$, giving $h_x=U/K_b$ wherever $h>0$. Downstream the uniform interior carries $q=Q$, so

$$
\boxed{h_\mathrm{int}=\frac QU,\qquad x_-=-\frac{K_bQ}{U^2},\qquad
h_\mathrm{up}(x)=\frac U{K_b}(x-x_-)\quad(x_-\le x\le0).}
$$

The upstream [volume flux](../../../../../volumetric-flow-rate.md) vanishes even though local [Darcy velocity](../../../../../darcy-velocity.md) contributions from background flow and [buoyancy](../../../../../buoyancy.md) cancel. The upstream stored volume is $\phi h_\mathrm{int}|x_-|/2$, a finite constant. The downstream plateau therefore extends a distance $ut+O(\ell_c)$, and its front advances at $u$ to leading order.

The [diffusive nose of an advected porous gravity current](../../../../../diffusive-nose-of-an-advected-porous-gravity-current.md) has width

$$
\boxed{w(t)\sim\sqrt{a h_\mathrm{int}t},\qquad
x_N(t)=ut+O\!\left(\sqrt{a h_\mathrm{int}t}\right)+O(\ell_c).}
$$

In a frame translating at $u$, balance the time derivative against the nonlinear gravity [diffusion](../../../../../diffusion.md). With $\eta=(x-x_c(t))/\sqrt{a h_\mathrm{int}t}$ and $x_c(t)=ut+O(\ell_c)$, the leading transition is $h=h_\mathrm{int}F(\eta)$, with

$$
(FF')'+\frac\eta2F'=0,\qquad F(-\infty)=1,\qquad F(\eta_N)=0.
$$

Its finite front has $F\sim(\eta_N/2)(\eta_N-\eta)$ as $\eta\uparrow\eta_N$. Independent numerical integration of this boundary-value problem gives $\eta_N\simeq1.23849$, so a more accurate leading nose position is $x_N\simeq x_c+1.23849\sqrt{a h_\mathrm{int}t}$ and its local shape is $F\simeq0.619247(1.23849-\eta)$. The entire transition has no elementary closed form. A useful explicit, approximate shape is the volume-preserving linear ramp

$$
\boxed{h\simeq h_\mathrm{int}\begin{cases}
1,&\eta\le-1,\\
(1-\eta)/2,&-1<\eta<1,\\
0,&\eta\ge1.
\end{cases}}
$$

This gives $x_N\simeq x_c+\sqrt{a h_\mathrm{int}t}$. Its ramp width is $2\sqrt{a h_\mathrm{int}t}$, and its edge obeys the exact [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) $\dot x_N=u-a h_x(x_N^-,t)$ to the displayed order. It also has the same area as a sharp step at $x_c$. This is an approximate ramp closure, not an exact solution of the nonlinear nose [ordinary differential equation](../../../../../ordinary-differential-equation.md). A constant phase shift $x_c=ut-|x_-|/2$ balances the finite upstream storage within this ramp approximation; the full solution's subleading matching may alter constant offsets.

For a rapid injection of total volume $V$, remove the source for $t>0$ and introduce $\xi=x-ut$. The [advected constant-volume porous gravity current](../../../../../advected-constant-volume-porous-gravity-current.md) obeys $h_t=a(hh_\xi)_\xi$ and $\int h\,d\xi=M=V/\phi$. A [similarity solution](../../../../../similarity-solution.md) has depth proportional to $t^{-1/3}$ and radius proportional to $t^{1/3}$. Direct substitution gives the compactly supported [Barenblatt solution](../../../../../barenblatt-solution.md)

$$
\boxed{h(x,t)=\frac{[R(t)^2-(x-ut)^2]_+}{6at},\qquad
R(t)=\left(\frac{9aVt}{2\phi}\right)^{1/3}.}
$$

Indeed $\int_{-R}^R(R^2-\xi^2)/(6at)\,d\xi=2R^3/(9at)=V/\phi$. Its centre translates at the pore speed $u$, its two edges are $ut\pm R(t)$, and its maximum depth decays as $t^{-1/3}$. The expression is exact for a point release within this reduced model; finite-width initial data approach this [similarity solution](../../../../../similarity-solution.md) at late times. If $U=0$, the constant-rate current remains in the symmetric spreading regime and the constant-volume solution has a stationary centre.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
