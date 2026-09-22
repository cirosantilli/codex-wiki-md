<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let the undisturbed water surface be $z=0$, the oil's upper surface $z=\eta(x,t)$ and its lower surface $z=b(x,t)$, so $h=\eta-b$. Leading [hydrostatic pressure](../../../../../hydrostatic-pressure.md) in the nearly inviscid water is $p_w=-\rho_wgz$ relative to atmospheric [pressure](../../../../../pressure.md); in the oil it is $p_H=\rho g(\eta-z)$. Equality at the interface gives $\rho gh=-\rho_wgb$, hence

$$
b=-\frac\rho{\rho_w}h,\qquad
\eta=\frac{\rho_w-\rho}{\rho_w}h.
$$

Thus the horizontal hydrostatic driving gradient is

$$
\boxed{p_{H,x}=\rho g\eta_x=\rho g'h_x,\qquad
 g'=\frac{\rho_w-\rho}{\rho_w}g.}
$$

This [reduced gravity](../../../../../reduced-gravity-split.md) accounts for most of the oil thickness being below the undisturbed water level.

Because the oil is much more viscous than the water and air, tangential tractions on both faces are negligible. In a thin layer, the leading horizontal [velocity](../../../../../velocity.md) is consequently independent of depth: the [floating extensional viscous gravity current](../../../../../floating-extensional-viscous-gravity-current.md) is a plug, rather than the parabolic profile of a no-slip gravity current. Integrating [incompressibility](../../../../../incompressible-flow.md) $u_x+w_z=0$ between the moving material boundaries, and using their [kinematic boundary condition](../../../../../kinematic-boundary-condition.md), gives conservation of oil volume,

$$
\boxed{h_t+(hu)_x=0,\qquad h_t+uh_x+hu_x=0.}
$$

To derive the factor $4$ in the extensional balance, [incompressibility](../../../../../incompressible-flow.md) gives $w_z=-u_x$. The [Newtonian fluid stress tensor](../../../../../newtonian-fluid-stress-tensor.md) has $\sigma_{zz}=-p-2\mu u_x$. Normal-stress balance relative to the hydrostatic part therefore requires $p=p_H-2\mu u_x$. The horizontal stress then satisfies

$$
\sigma_{xx}=-p+2\mu u_x=-p_H+4\mu u_x.
$$

Thus the longitudinal tensile [force](../../../../../force.md) in an oil slice, relative to its [hydrostatic pressure](../../../../../hydrostatic-pressure.md), is $4\mu hu_x$ per unit width. Balancing its difference across the slice with the horizontal driving [force](../../../../../force.md) $-hp_{H,x}\,dx$ yields

$$
\boxed{4\mu(hu_x)_x=hp_{H,x},\qquad
\frac{4\mu}{h}(hu_x)_x=p_{H,x}.}
$$

The coefficient is the planar extensional [Trouton ratio](../../../../../trouton-ratio.md), arising from both the direct horizontal strain and the [pressure](../../../../../pressure.md) correction required by the transverse normal-stress condition.

Using the [pressure gradient](../../../../../pressure-gradient.md) above, integration in $x$ gives

$$
4\mu hu_x=\frac12\rho g'h^2+C(t).
$$

The stated nose stress condition sets $C(t)=0$, not an arbitrary imposed inlet tension. Consequently

$$
u_x=kh,\qquad k=\frac{\rho g'}{8\mu}.
$$

For a material slice injected at time $t_0$, let $\tau=t-t_0$ be its age. The thickness equation along its [Lagrangian trajectory](../../../../../lagrangian-trajectory.md) is $dh/dt=-hu_x=-kh^2$, with $h=h_0$ at injection. Define

$$
T=\frac1{kh_0}=\frac{8\mu}{\rho g'h_0}.
$$

Then $h=h_0/(1+\tau/T)$. The slice injected during $dt_0$ has volume $h_0u_0dt_0$ per unit width, so at fixed observation time $t$,

$$
-h\frac{\partial x}{\partial t_0}=h_0u_0,
\qquad
\frac{\partial x}{\partial\tau}=u_0\left(1+\frac\tau T\right).
$$

Since a newly injected slice has $x(t,t)=0$, integration and subsequent differentiation along a material slice give the [constant-flux floating extensional gravity current](../../../../../constant-flux-floating-extensional-gravity-current.md):

$$
\boxed{h(t;t_0)=\frac{h_0}{1+(t-t_0)/T},\qquad
u(t;t_0)=u_0\left(1+\frac{t-t_0}{T}\right),\qquad
x(t;t_0)=u_0\left[(t-t_0)+\frac{(t-t_0)^2}{2T}\right].}
$$

The oldest slice forms the nose. Measuring time from the start of injection, $t_0=0$ there, so

$$
\boxed{x_N(t)=u_0t+\frac{\rho g'h_0u_0}{16\mu}t^2,\qquad
h_N(t)=\frac{h_0}{1+t/T}.}
$$

Its speed $\dot x_N=u_0(1+t/T)$ is exactly the material [velocity](../../../../../velocity.md) at the nose, as required.

For a fixed position $x$ behind the nose, the age needed to reach it is determined by $x/u_0=\tau+\tau^2/(2T)$, independently of the observation time. Hence both thickness and [velocity](../../../../../velocity.md) become stationary there once the nose has passed. Eliminating $\tau$ gives

$$
\boxed{h(x)=h_0\left(1+\frac{\rho g'h_0x}{4\mu u_0}\right)^{-1/2},\qquad
u(x)=u_0\left(1+\frac{\rho g'h_0x}{4\mu u_0}\right)^{1/2}.}
$$

Their product is $h_0u_0$, so the steady profile carries precisely the inlet [volume flux](../../../../../volumetric-flow-rate.md); integrating it to $x_N(t)$ gives the total injected volume $h_0u_0t$.

The length

$$
\boxed{\ell=\frac{\mu u_0}{\rho g'h_0}}
$$

is the horizontal distance over which reduced-gravity driving causes an order-one change in inlet speed and thickness by viscous extension. The associated age is $T=8\ell/u_0$; the exact profile contains $x/(4\ell)$. It is an extensional adjustment length, not a shear-diffusion scale. The result applies while the stated thin-layer and negligible-inertia approximations remain valid.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
