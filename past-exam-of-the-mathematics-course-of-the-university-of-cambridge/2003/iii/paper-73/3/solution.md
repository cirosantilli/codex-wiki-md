<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $z$ measure height above the substrate, and write $\mu=\rho\nu$. In the [lubrication approximation](../../../../../lubrication-theory.md), the horizontal scale $\ell$ is much larger than the typical height $H_0$. Vertical momentum balance is hydrostatic to leading order, while the horizontal balance retains the dominant vertical shear:

$$
p=p_{\rm atm}+\rho g(h-z),\qquad \mu u_{zz}=p_x=\rho g h_x.
$$

The [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) gives $u(0)=0$; negligible air viscosity and constant [surface tension](../../../../../surface-tension.md) give $u_z(h)=0$. Integrating twice and then through the depth yields

$$
u(x,z,t)=\frac{g h_x}{\nu}\left(\frac{z^2}{2}-hz\right),\qquad
q=\int_0^hu\,dz=-\frac{g}{3\nu}h^3h_x.
$$

The free-surface [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) and [incompressibility](../../../../../incompressible-flow.md) imply $h_t+q_x=0$. Therefore

$$
\boxed{h_t=\frac{g}{3\nu}(h^3h_x)_x.}
$$

The cross-sectional area $A=\int h\,dx$ is conserved when the endpoint [volume flux](../../../../../volumetric-flow-rate.md) vanishes.

The relevant small groups follow from the same balances. Put $\epsilon_h=H_0/\ell$ and $U_*=gH_0^3/(3\nu\ell)$. Small $\epsilon_h$ suppresses horizontal viscous derivatives and makes vertical viscous corrections to hydrostatic pressure smaller by $O(\epsilon_h^2)$. The ratio of horizontal inertia to vertical viscous stress is

$$
\boxed{\frac{U_*H_0^2}{\nu\ell}=\epsilon_h\mathrm{Re}_{H_0}
=\epsilon_h^2\mathrm{Re}_{\ell}\ll1.}
$$

Thus a small full-length [Reynolds number](../../../../../reynolds-number.md) is sufficient but not necessary: thin-layer geometry reduces the inertial ratio. The unsteady viscous ratio $H_0^2/(\nu t_*)$ must likewise be small; on the spreading timescale $t_*=\ell/U_*$ it equals the displayed group. If [surface tension](../../../../../surface-tension.md) is retained, its pressure-gradient correction relative to gravity is

$$
\boxed{\frac{\gamma}{\rho g\ell^2}=\mathrm{Bo}_{\ell}^{-1}\ll1.}
$$

The [Bond number](../../../../../bond-number.md) here uses the horizontal scale, because the capillary pressure is $O(\gamma H_0/\ell^2)$ whereas the hydrostatic pressure is $O(\rho gH_0)$. We also neglect air shear and evaporation and assume a Newtonian fluid with constant [kinematic viscosity](../../../../../kinematic-viscosity.md).

To find the [similarity solution](../../../../../similarity-solution.md), put $K=g/(3\nu)$. Conservation of $A$ gives $h\sim A/\ell$, and balancing the [time derivative](../../../../../time-derivative.md) against the nonlinear diffusion gives $\ell^5\sim KA^3t$. A normalized ansatz is

$$
h=\left(\frac{A^2}{Kt}\right)^{1/5}f(\xi),\qquad
\xi=\frac{x-x_c}{(KA^3t)^{1/5}},\qquad \int f\,d\xi=1.
$$

Substitution gives $(f^3f')'=-(f+\xi f')/5$. For the symmetric zero-flux profile, one integration gives $f^3f'=-\xi f/5$, and on its positive support a second integration gives

$$
f^3=C-3\xi^2/10.
$$

Thus the solution is a compactly supported [Barenblatt solution](../../../../../barenblatt-solution.md) of the [porous medium equation](../../../../../porous-medium-equation.md). Let $\ell(t)$ denote its half-width. In dimensional variables,

$$
\boxed{h(x,t)=\left[\frac{9\nu}{10gt}\{\ell(t)^2-(x-x_c)^2\}\right]_+^{1/3}.}
$$

Here the positive-part notation sets the height to zero outside $|x-x_c|<\ell$. The area normalization fixes the coefficient, not merely the exponent. With $x-x_c=\ell\sin\theta$,

$$
A=2\left(\frac{9\nu}{10gt}\right)^{1/3}\ell^{5/3}
\int_0^{\pi/2}\cos^{5/3}\theta\,d\theta.
$$

Writing the remaining integral as $I$, the final widths are

$$
\boxed{\ell(t)=\left(\frac{5gA^3t}{36\nu I^3}\right)^{1/5},\qquad
\text{full drop width}=2\left(\frac{5gA^3t}{36\nu I^3}\right)^{1/5}.}
$$

The height falls like $t^{-1/5}$ and the width grows like $t^{1/5}$. The [volume flux](../../../../../volumetric-flow-rate.md) tends to zero at the front, even though the profile slope diverges; this gives a valid compactly supported [weak solution](../../../../../weak-solution.md) of the reduced equation. The diverging edge slope means the [lubrication approximation](../../../../../lubrication-theory.md) is not uniform at a microscopic contact line. Surface-tension or contact-line physics supplies an inner regularization without changing the gravity-dominated bulk similarity law in its validity regime. This is an exact source-type solution for $t>0$; an arbitrary finite initial drop approaches an appropriate late-time profile rather than being exactly represented by this singular initial profile.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
