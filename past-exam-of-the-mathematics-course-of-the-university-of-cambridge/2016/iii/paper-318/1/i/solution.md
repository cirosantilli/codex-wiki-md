<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [fully developed flow](../../../../../../fully-developed-flow.md) branch of [Hartmann flow](../../../../../../hartmann-flow.md). Translation invariance along the walls makes the velocity and induced [magnetic field](../../../../../../magnetic-field.md) functions of $z$ alone. [Incompressible flow](../../../../../../incompressible-flow.md) and zero normal velocity at the walls give $u_z'=0$ and hence $u_z=0$. The zero [divergence](../../../../../../divergence.md) of the [magnetic field](../../../../../../magnetic-field.md) makes $B_z$ constant, equal to the imposed $B_0$. There is no forcing in $y$; the homogeneous $y$-components obey the same coupled viscous-resistive equations as the $x$-components, with zero boundary data. Multiplying them by $u_y$ and $b_y/(\mu_0\rho)$, integrating by parts and adding gives

$$
\nu\int_{-L}^{L}(u_y')^2\,dz+\frac\eta{\mu_0\rho}\int_{-L}^{L}(b_y')^2\,dz=0.
$$

Thus $u_y=b_y=0$, establishing the asserted forms on this [fully developed flow](../../../../../../fully-developed-flow.md) branch. This is a symmetry reduction of the steady channel model, rather than a claim that every possible flow in a channel is translation invariant.

The [current density](../../../../../../current-density.md) and [Lorentz force density](../../../../../../lorentz-force-density.md) are

$$
\mathbf J=\frac1{\mu_0}\nabla\times\mathbf B=(0,b'/\mu_0,0),
\qquad \mathbf J\times\mathbf B=\frac1{\mu_0}(B_0b',0,-bb').
$$

The advective acceleration vanishes because $\mathbf u\cdot\nabla=u(z)\partial_x$ acts on fields independent of $x$. The $x$-component of the [magnetohydrodynamic momentum equation](../../../../../../magnetohydrodynamic-momentum-equation.md) therefore gives

$$
\boxed{0=G+\frac{B_0}{\mu_0\rho}b'+\nu u''.}
$$

The $z$-component must also balance: it requires $\partial_z(p+b^2/(2\mu_0))=0$. Hence a compatible [pressure](../../../../../../pressure.md) is $p(x,z)=p_*-\rho Gx-b(z)^2/(2\mu_0)$; the specified streamwise [pressure gradient](../../../../../../pressure-gradient.md) does not require the ordinary pressure to be uniform in $z$. This accounts for the [magnetic pressure](../../../../../../magnetic-pressure.md) of the induced field.

The [resistive induction equation](../../../../../../resistive-induction-equation.md) with constant [magnetic diffusivity](../../../../../../magnetic-diffusivity.md) gives $\partial_t\mathbf B=\nabla\times(\mathbf u\times\mathbf B)+\eta\nabla^2\mathbf B$. Since $\mathbf u\times\mathbf B=(0,-B_0u,0)$, its [curl](../../../../../../curl.md) has $x$-component $B_0u'$. Steadiness consequently gives

$$
\boxed{0=B_0u'+\eta b''.}
$$

Finally the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) gives $u(\pm L)=0$, and the [normal magnetic field boundary condition](../../../../../../normal-magnetic-field-boundary-condition.md) gives $b(\pm L)=0$. **The coupled equations and all wall conditions follow directly from momentum balance and magnetic induction.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
