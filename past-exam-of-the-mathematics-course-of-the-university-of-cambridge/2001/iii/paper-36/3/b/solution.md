<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $K$ be the [kinetic energy](../../../../../../kinetic-energy.md), $M$ the [magnetic energy](../../../../../../magnetic-energy.md) and $E=K+M$:

$$
K=\frac\rho2\int_D|\mathbf v|^2\,dV,\qquad M=\frac1{2\mu_0}\int_D|\mathbf B|^2\,dV.
$$

Dot the [magnetohydrodynamic momentum equation](../../../../../../magnetohydrodynamic-momentum-equation.md) with $\mathbf v$ and integrate. [Incompressibility](../../../../../../incompressible-flow.md) and the zero boundary [velocity](../../../../../../velocity.md) remove the advective and [pressure](../../../../../../pressure.md) work. The viscous term integrates to $-\rho\nu\int_D|\nabla\mathbf v|^2$. Thus

$$
\dot K=\int_D\mathbf v\cdot(\mathbf j\times\mathbf B)\,dV-\rho\nu\int_D|\nabla\mathbf v|^2\,dV.
$$

The [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) gives, with no boundary contribution,

$$
\dot M=\frac1{\mu_0}\int_D\mathbf B\cdot\nabla\times(\mathbf v\times\mathbf B)\,dV=-\int_D\mathbf v\cdot(\mathbf j\times\mathbf B)\,dV.
$$

The [Lorentz force density](../../../../../../lorentz-force-density.md) therefore transfers energy between the field and the fluid without creating total energy. Since $\nabla\cdot\mathbf v=0$ and $\mathbf v=0$ on the boundary, another [integration by parts](../../../../../../integration-by-parts.md) gives $\int|\nabla\mathbf v|^2=\int|\boldsymbol\omega_v|^2$, where $\boldsymbol\omega_v=\nabla\times\mathbf v$ is [vorticity](../../../../../../vorticity.md). The [viscous magnetic-relaxation energy identity](../../../../../../viscous-magnetic-relaxation-energy-identity.md) is

$$
\boxed{\frac{dE}{dt}=-\rho\nu\int_D|\boldsymbol\omega_v|^2\,dV,\qquad E(0)=\frac1{2\mu_0}\int_D|\mathbf B_0|^2\,dV.}
$$

The conserved nonzero [magnetic helicity](../../../../../../magnetic-helicity.md) prevents all the field energy from disappearing. Fix a bounded inverse-curl convention for the [magnetic vector potential](../../../../../../magnetic-vector-potential.md), so that $\|\mathbf A\|_2\leq C_D\|\mathbf B\|_2$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives the [magnetic-energy lower bound from helicity](../../../../../../magnetic-energy-lower-bound-from-helicity.md),

$$
M\geq\frac{|H_M|}{2\mu_0C_D}>0.
$$

Consequently $E$ decreases to a finite positive limit and

$$
\rho\nu\int_0^\infty\|\boldsymbol\omega_v(t)\|_2^2,dt=E(0)-E_\infty<\infty.
$$

Under the intended regular long-time interpretation of smooth [vorticity](../../../../../../vorticity.md), the dissipation cannot keep producing peaks of fixed height and arbitrarily short duration. More precisely, if $d(t)=\|\boldsymbol\omega_v(t)\|_2^2$ is [uniformly continuous](../../../../../../uniform-continuity.md), [uniformly continuous integrable dissipation tends to zero](../../../../../../uniformly-continuous-integrable-dissipation-tends-to-zero.md) proves $d(t)\to0$. The [Poincaré inequality](../../../../../../poincare-inequality.md) and the identity above then imply $\|\mathbf v(t)\|_2\to0$.

To identify the asymptotic state, suppose the regular relaxation has a limit, or work on a compact invariant limiting set on which the energy is continuous. On such a set the energy is constant, so the displayed identity forces $\boldsymbol\omega_v=0$, and the zero boundary [velocity](../../../../../../velocity.md) forces $\mathbf v=0$. The induction equation is then stationary, and the momentum equation becomes

$$
\boxed{\mathbf j_\infty\times\mathbf B_\infty=\nabla p_\infty,\qquad \nabla\cdot\mathbf B_\infty=0,\qquad \mathbf B_\infty\cdot\mathbf n=0.}
$$

This is [magnetostatic equilibrium](../../../../../../magnetostatic-equilibrium.md), with nonzero field allowed and required here by conserved [magnetic helicity](../../../../../../magnetic-helicity.md). It is not necessarily a [force-free magnetic field](../../../../../../force-free-magnetic-field.md): a [pressure gradient](../../../../../../pressure-gradient.md) can balance the magnetic force. If the field develops a [current sheet](../../../../../../current-sheet.md), equilibrium is understood with the corresponding interface force balance.

There is a mathematical qualification to the smoothness premise. Smoothness at each finite time alone does not prove uniform long-time bounds, uniform continuity of dissipation or convergence to one limiting field. The energy calculation proves finite total dissipation unconditionally for a smooth solution; the settling conclusion is the regular-relaxation argument just given. A rigorous global convergence theorem requires that additional long-time control. In particular, smooth [vorticity](../../../../../../vorticity.md) does not require smooth [electric current density](../../../../../../current-density.md) in the limiting state.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
