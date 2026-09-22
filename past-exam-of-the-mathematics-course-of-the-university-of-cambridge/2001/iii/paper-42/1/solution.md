<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume [axisymmetry](../../../../../axisymmetric-vector-field.md) in a [thin disk](../../../../../thin-disk.md) orbiting a fixed central [mass](../../../../../mass.md) $M$. To leading order in thickness, the [Keplerian rotation](../../../../../keplerian-disk.md) is independent of height, $\Omega=(GM/r^3)^{1/2}$, with slow radial drift compared with $r\Omega$. Neglect radial [pressure](../../../../../pressure.md) support in the orbital balance, changes in the central potential, mass loss through the disk surfaces and applied surface [torques](../../../../../torque.md). The [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) can represent viscous or effective turbulent/magnetic transport; only its vertically integrated azimuthal component enters the [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) equation.

Define the [surface density](../../../../../surface-density-of-a-disk.md) and its mass-weighted radial [velocity](../../../../../velocity.md) by

$$
\Sigma=\int\rho\,dz,\qquad\Sigma\bar u_r=\int\rho u_r\,dz,
$$

and set $W_{r\phi}=\int T_{r\phi}\,dz$. Integrating [mass conservation](../../../../../mass-conservation.md) vertically gives

$$
\partial_t\Sigma+\frac1r\partial_r(r\Sigma\bar u_r)=0.
$$

The azimuthal equation in [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md), multiplied by $r$ and combined with [mass conservation](../../../../../mass-conservation.md), is the conservative equation for [specific angular momentum](../../../../../specific-angular-momentum.md) $l=r^2\Omega$. The cylindrical [stress tensor](../../../../../cauchy-stress-tensor.md) [divergence](../../../../../divergence.md) contributes $r^{-1}\partial_r(r^2T_{r\phi})+\partial_z(rT_{\phi z})$. With vanishing surface [torque](../../../../../torque.md), vertical integration therefore gives

$$
\partial_t(\Sigma l)+\frac1r\partial_r(r\Sigma\bar u_r l)
=\frac1r\partial_r(r^2W_{r\phi}).
$$

Because $l(r)$ is fixed in time, subtracting $l$ times the mass equation yields

$$
\Sigma\bar u_r\frac{dl}{dr}=\frac1r\partial_r(r^2W_{r\phi}).
$$

Define the [effective viscosity defined by disk stress](../../../../../effective-viscosity-defined-by-disk-stress.md) by

$$
\boxed{\bar\nu\Sigma r\frac{d\Omega}{dr}=W_{r\phi},\qquad
\bar\nu=-\frac{2}{3\Sigma\Omega}\int T_{r\phi}\,dz\quad\text{for Keplerian rotation}.}
$$

This sign convention treats $T_{r\phi}$ as the [shear stress](../../../../../shear-stress.md) appearing with $+\nabla\cdot\mathbf T$. For the [Newtonian fluid stress tensor](../../../../../newtonian-fluid-stress-tensor.md) it reduces to the [density-weighted viscosity of a disk](../../../../../density-weighted-viscosity-of-a-disk.md), $\bar\nu=\Sigma^{-1}\int\rho\nu dz$, rather than an unweighted height average.

Using $l=\sqrt{GMr}$ and $W_{r\phi}=-(3/2)\bar\nu\Sigma\Omega$ in the [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) equation gives

$$
\bar u_r=-\frac3{\Sigma\sqrt r}\partial_r(\sqrt r\bar\nu\Sigma).
$$

Substitution into [mass conservation](../../../../../mass-conservation.md) proves the [Keplerian viscous diffusion equation](../../../../../keplerian-viscous-diffusion-equation.md):

$$
\boxed{\partial_t\Sigma=\frac3r\partial_r\left[\sqrt r\,\partial_r(\sqrt r\bar\nu\Sigma)\right].}
$$

The outward [viscous torque in an accretion disk](../../../../../viscous-torque-in-an-accretion-disk.md) is $\mathcal G=-2\pi r^2W_{r\phi}=3\pi\sqrt{GM}\sqrt r\bar\nu\Sigma$.

For $\bar\nu=Ar$ with $A>0$, make the [heat-equation transform for linear-radius disk viscosity](../../../../../heat-equation-transform-for-linear-radius-disk-viscosity.md)

$$
\boxed{x=2\sqrt{\frac r{3A}},\qquad g=\sqrt r\bar\nu\Sigma=Ar^{3/2}\Sigma.}
$$

Writing $y=\sqrt r$, the diffusion equation becomes $g_t=(3A/4)g_{yy}$; the displayed rescaling of $y$ gives exactly $\boxed{g_t=g_{xx}}$, with the original time unchanged. The [torque](../../../../../torque.md) is $3\pi\sqrt{GM}g$, so the [zero-torque inner boundary condition](../../../../../zero-torque-inner-boundary-condition.md) at the origin becomes $g(0,t)=0$ on the half-line $x>0$.

A positive [similarity solution](../../../../../similarity-solution.md) obeying this [boundary condition](../../../../../boundary-condition.md) is

$$
\boxed{g=Cxt^{-3/2}e^{-x^2/(4t)},\qquad
\Sigma=\frac{2C}{A\sqrt{3A}}\frac{t^{-3/2}}r e^{-r/(3At)},\qquad C>0.}
$$

For example, substitution of $g=t^{-1}F(x/\sqrt t)$ reduces the [heat equation](../../../../../heat-equation.md) to $F''+(\eta/2)F'+F=0$, and $F=C\eta e^{-\eta^2/4}$ satisfies it and vanishes at zero. A replacement of $t$ by $t+t_0$ gives a finite-mass initial profile at time zero if desired.

To determine the global integrals, transform the [mass](../../../../../mass.md) and [angular momentum](../../../../../angular-momentum.md):

$$
M_d=2\pi\int_0^\infty\Sigma r\,dr=2\pi\sqrt{\frac3A}\int_0^\infty g\,dx,
\qquad
J_d=2\pi\sqrt{GM}\int_0^\infty\Sigma r^{3/2}dr=3\pi\sqrt{GM}\int_0^\infty xg\,dx.
$$

The [Gaussian integrals](../../../../../gaussian-integral.md) give

$$
\boxed{M_d=4\pi C\sqrt{3/A}\,t^{-1/2},\qquad
J_d=6\pi^{3/2}C\sqrt{GM}=\text{constant}.}
$$

Thus the [accreting similarity disk with viscosity proportional to radius](../../../../../accreting-similarity-disk-with-viscosity-proportional-to-radius.md) loses [mass](../../../../../mass.md) as $t^{-1/2}$ while conserving [angular momentum](../../../../../angular-momentum.md); its characteristic radius grows proportional to $At$. The accretion rate at the origin is $-\dot M_d=2\pi C\sqrt{3/A}\,t^{-3/2}$. Its radial [velocity](../../../../../velocity.md) $\bar u_r=r/t-3A/2$ shows inward flow at small radius and outward spreading at large radius. The integrable inner [density](../../../../../density.md) singularity is part of the idealized extension to $r=0$.

For the other profile, direct differentiation gives

$$
\frac{g_t}{g}=-\frac1{2t}+\frac{x^2}{4t^2}=\frac{g_{xx}}g,
\qquad g=t^{-1/2}e^{-x^2/(4t)}.
$$

It also satisfies the [heat equation](../../../../../heat-equation.md), but has $g(0,t)=t^{-1/2}\ne0$ and $g_x(0,t)=0$. It therefore has a nonzero inner [torque](../../../../../torque.md) and zero mass flow at the origin, not the previous [zero-torque inner boundary condition](../../../../../zero-torque-inner-boundary-condition.md). Here

$$
\Sigma=\frac{t^{-1/2}}{Ar^{3/2}}e^{-r/(3At)},\qquad
\bar u_r=\frac rt,
$$



$$
\boxed{M_d=2\pi\sqrt{3\pi/A}=\text{constant},\qquad
J_d=6\pi\sqrt{GM}\,t^{1/2},\qquad
\mathcal G(0,t)=\dot J_d=3\pi\sqrt{GM}\,t^{-1/2}.}
$$

An arbitrary positive amplitude multiplies these quantities. This [constant-mass disk with viscosity proportional to radius](../../../../../constant-mass-disk-with-viscosity-proportional-to-radius.md) spreads outward under a central [torque](../../../../../torque.md) that supplies [angular momentum](../../../../../angular-momentum.md), with no ongoing central mass supply. It has the reflecting [Neumann boundary condition](../../../../../neumann-boundary-condition.md) for the [heat equation](../../../../../heat-equation.md) and can be regarded as the spreading of an initially central mass distribution driven by an applied [torque](../../../../../torque.md). It is distinct from the accreting zero-torque solution; the ideal origin does not model a finite stellar surface or a relativistic inner disk.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
