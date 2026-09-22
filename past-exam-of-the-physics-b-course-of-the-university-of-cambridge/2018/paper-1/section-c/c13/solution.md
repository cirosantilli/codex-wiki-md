<h1 id="section-c/c13/solution">Solution</h1>

↑ **Parent:** [C13](../c13.md)

**Meaning and microscopic origin.** For a [Newtonian fluid](../../../../../newtonian-fluid.md), the [dynamic viscosity](../../../../../dynamic-viscosity-split.md) $\eta$ measures tangential momentum transfer between fluid layers moving at different speeds. For the Newtonian shear considered here, $\tau_{xz}=\eta\,dv_z/dx$, with units $\mathrm{Pa\,s}$ for $\eta$. Molecular motion and collisions transport momentum across layers in a gas; intermolecular interactions contribute strongly in liquids. The resulting viscous forces oppose relative shear motion and convert organized kinetic energy to heat. The constitutive law is Newtonian and isotropic; incompressibility alone does not establish it.

**Vertical force balance.** Choose $z$ downward, as in the original diagram, and $x$ outward normal to the plate. In a uniform steady film, $\mathbf v=v_z(x)\widehat{\mathbf z}$ has zero advective acceleration and no along-plate [pressure gradient](../../../../../pressure-gradient.md). On a slice of thickness $dx$, the net shear force per unit face area is $\tau(x+dx)-\tau(x)$, while its weight per unit area is $\rho g\,dx$. Therefore

$$
\boxed{d\tau=-\rho g\,dx.}
$$

Here $\tau=\eta\,dv_z/dx$ denotes the downward traction on a face with positive $x$ normal. The opposite face has the opposite traction orientation, accounting for the sign in the force difference.

**Boundary conditions.** At the fixed solid wall, the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) is $v_z(0)=0$, with no normal penetration. At the free surface $x=d$, neglect air shear, so $\tau(d)=0$ and hence $v_z'(d)=0$. The flat [free surface](../../../../../free-surface.md) has normal pressure $p_{\rm atm}$, neglecting surface-curvature effects. These are a velocity condition at the wall and a stress condition at the free surface, not zero velocity at both boundaries.

**The parabolic speed profile.** Integrating $\tau'=-\rho g$ from the shear-free surface gives $\tau(x)=\rho g(d-x)$. Thus

$$
\eta\frac{dv_z}{dx}=\rho g(d-x),
$$

and the wall condition yields

$$
\boxed{v_z(x)=\frac{\rho g}{\eta}\left(dx-\frac{x^2}{2}\right)
=ax+bx^2,\qquad
a=\frac{\rho gd}{\eta},\quad b=-\frac{\rho g}{2\eta}.}
$$

It is zero at the wall and largest at the free surface, where its gradient vanishes. The wall shear $\rho gd$ supports the downslope weight of the film per unit plate area.

**Volume flux per unit width.** Integrate through the depth:

$$
q=\int_0^d v_z(x)\,dx
=\frac{\rho g}{\eta}\left(\frac{d^3}{2}-\frac{d^3}{6}\right),
\qquad
\boxed{q=\frac{\rho gd^3}{3\eta}.}
$$

This is volume flow per unit length in $y$, with units $\mathrm{m^2\,s^{-1}}$.

**Inclining the plate.** Keep $x$ normal outward from the plate and use $s$ downslope. The gravitational components are $g\sin\theta$ downslope and $-g\cos\theta$ normal to the plate. For a uniform film of normal thickness $d$, the steady slice equations are

$$
0=-\frac{\partial p}{\partial x}-\rho g\cos\theta,\qquad
0=-\frac{\partial p}{\partial s}+\rho g\sin\theta
+\eta\frac{d^2v}{dx^2}.
$$

The free-surface pressure condition gives

$$
p(x)=p_{\rm atm}+\rho g\cos\theta(d-x).
$$

Uniform $d$ makes $\partial_sp=0$. The same no-slip and zero-surface-shear conditions then give the [uniform gravity-driven Newtonian film](../../../../../uniform-gravity-driven-newtonian-film.md),

$$
\boxed{v(x)=\frac{\rho g\sin\theta}{\eta}
\left(dx-\frac{x^2}{2}\right).}
$$

The component normal to the plate changes the hydrostatic pressure, while the tangential component drives the flow. The thickness is measured normal to the tilted plate.

**The inclined-film volume flux.** Integrating the new profile gives

$$
\boxed{q(\theta)=\frac{\rho gd^3}{3\eta}\sin\theta.}
$$

It recovers the vertical result at $\theta=\pi/2$ and vanishes on a horizontal plate at fixed uniform depth. A varying depth, imposed pressure gradient or significant air shear would require additional terms; the solution here uses the uniform film specified by the simple draining-plate model.

## ↑ Ancestors (14)

1. [C13](../c13.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
