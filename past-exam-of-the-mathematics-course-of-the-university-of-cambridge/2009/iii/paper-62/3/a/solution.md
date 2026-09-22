<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an isolated [collisionless stellar system](../../../../../../collisionless-stellar-system.md), define the scalar second mass moment and total [kinetic energy](../../../../../../kinetic-energy.md) by

$$
I(t)=\int\rho(\boldsymbol r,t)r^2\,d^3r,
\qquad T=\frac12\int f(\boldsymbol r,\boldsymbol v,t)v^2\,d^3r\,d^3v.
$$

Take moments of the [Collisionless Boltzmann equation](../../../../../../collisionless-boltzmann-equation.md), with vanishing surface fluxes. For any time-independent phase-space function $A$, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\frac d{dt}\int fA\,d^3r\,d^3v
=\int f\left(\boldsymbol v\cdot\nabla_r A-\nabla\phi\cdot\nabla_v A\right)d^3r\,d^3v.
$$

Apply this first to $A=r^2$ and then to $A=\boldsymbol r\cdot\boldsymbol v$. The result is

$$
\dot I=2\int f\boldsymbol r\cdot\boldsymbol v\,d^3r\,d^3v,
\qquad\frac12\ddot I=2T-\int\rho\boldsymbol r\cdot\nabla\phi\,d^3r.
$$

The potential is self-consistent Newtonian gravity, so

$$
\phi(\boldsymbol r)=-G\int\frac{\rho(\boldsymbol r')}{|\boldsymbol r-\boldsymbol r'|}\,d^3r',
\qquad W=-\frac G2\iint\frac{\rho(\boldsymbol r)\rho(\boldsymbol r')}{|\boldsymbol r-\boldsymbol r'|}\,d^3r\,d^3r'.
$$

Symmetrize the force integral under $\boldsymbol r\leftrightarrow\boldsymbol r'$:

$$
\begin{aligned}
\int\rho\boldsymbol r\cdot\nabla\phi\,d^3r
&=\frac G2\iint\rho\rho'\frac{(\boldsymbol r-\boldsymbol r')\cdot(\boldsymbol r-\boldsymbol r')}{|\boldsymbol r-\boldsymbol r'|^3}\,d^3r\,d^3r'\\
&=\frac G2\iint\frac{\rho\rho'}{|\boldsymbol r-\boldsymbol r'|}\,d^3r\,d^3r'=-W.
\end{aligned}
$$

Thus the dynamical [virial theorem](../../../../../../virial-theorem.md) is $\ddot I/2=2T+W$. For a steady system, $\ddot I=0$, and consequently

$$
\boxed{2T+W=0.}
$$

For bounded statistically steady motion, averaging instead gives $2\langle T\rangle+\langle W\rangle=0$ provided $[\dot I(\tau)-\dot I(0)]/\tau\to0$. Collisionlessness alone does not imply instantaneous [virial equilibrium](../../../../../../virial-equilibrium.md): a collapsing system retains the $\ddot I$ term. The displayed derivation assumes a finite second mass moment, or a limiting version with vanishing boundary terms, and no confining boundary-pressure contribution.

In [virial equilibrium](../../../../../../virial-equilibrium.md), the total [energy](../../../../../../energy.md) is $E_{\rm tot}=T+W=-T$. Define the kinetic [temperature](../../../../../../temperature.md) $\Theta$ at fixed particle number $N$ by $T=3Nk_B\Theta/2$. Along an equilibrium sequence,

$$
\boxed{\frac{dE_{\rm tot}}{d\Theta}=-\frac32Nk_B<0.}
$$

This is the [negative heat capacity of a virialized gravitational system](../../../../../../negative-heat-capacity-of-a-virialized-gravitational-system.md): removing total energy makes the kinetic temperature rise. A [collisionless stellar system](../../../../../../collisionless-stellar-system.md) need not be in thermal equilibrium, so without that additional assumption this is a kinetic-temperature interpretation of [heat capacity](../../../../../../heat-capacity.md), rather than an assertion that every stellar distribution has a thermodynamic temperature.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
