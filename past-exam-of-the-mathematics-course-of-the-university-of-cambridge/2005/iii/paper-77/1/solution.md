<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [Newtonian fluid](../../../../../newtonian-fluid.md), write $\boldsymbol\sigma=-pI+2\mu e$, where $e=(\nabla u+\nabla u^T)/2$ is the [rate-of-strain tensor](../../../../../strain-rate-tensor.md). The [Stokes equation](../../../../../stokes-equation.md) without body force gives $\partial_j\sigma_{ij}=0$. Since the [stress tensor](../../../../../cauchy-stress-tensor.md) is symmetric, its contraction with the antisymmetric part of the velocity gradient is zero. Thus

$$
\partial_j(u_i\sigma_{ij})=\sigma_{ij}\partial_ju_i=\boldsymbol\sigma:e.
$$

The [divergence theorem](../../../../../divergence-theorem.md) proves the boundary-work identity

$$
\boxed{D=\int_V\boldsymbol\sigma:e\,dV=\int_{\partial V}u\cdot\boldsymbol\sigma n\,dS.}
$$

For an [incompressible flow](../../../../../incompressible-flow.md), $\operatorname{tr}e=0$, so $D=2\mu\int_V e:e\,dV\geq0$ is precisely the [viscous dissipation](../../../../../viscous-dissipation.md).

Apply this identity to the particle-free volume and then to the fluid outside the added particle. On the rigid particle, the velocity has the form $V+\Omega\times x$. Its contribution to the boundary work is $V\cdot F+\Omega\cdot T$, which vanishes because the particle is [force-free](../../../../../force-free.md) and [torque-free](../../../../../torque-free.md). The outer velocity is unchanged. Subtracting the two boundary-work identities therefore gives

$$
\boxed{D'=\int_{\partial V_0}U_0\cdot\boldsymbol\sigma'n\,dS.}
$$

To move this expression to the particle surface, apply the [Lorentz reciprocal theorem](../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) to $(u_0,\sigma_0)$ and $(u',\sigma')$ in the punctured fluid domain. For completeness, its local proof is

$$
\nabla\cdot(u_0\cdot\sigma'-u'\cdot\sigma_0)
=2\mu e_0:e'-2\mu e':e_0=0.
$$

On the outer boundary $u'=0$. Let $N=-n$ be the particle-outward normal, opposite to the fluid-outward normal there. Integrating the preceding divergence identity gives

$$
\boxed{D'=\int_A(u_0\cdot\sigma'-u'\cdot\sigma_0)N\,dS.}
$$

This expression includes the removal of the original fluid inside the particle; that removal must not be counted separately again.

For a [sphere in a uniform straining Stokes flow](../../../../../sphere-in-a-uniform-straining-stokes-flow.md), $E$ is symmetric and trace free, and $u_0=Ex$. Symmetry gives zero rigid translation and rotation. Put $H=x\cdot Ex$ and $r=|x|$. Use the [Unscaled Papkovich–Neuber representation](../../../../../unscaled-papkovich-neuber-representation.md) printed on the paper, with the decaying harmonic potentials

$$
\Phi'=C\frac{a^3Ex}{r^3},\qquad \chi'=B\frac{a^5H}{r^5}.
$$

Their harmonicity follows from $x_i/r^3=-\partial_i(1/r)$ and from $H/r^5$ being a trace-free second derivative of $1/r$. Direct differentiation gives

$$
u'=-3C\frac{a^3H x}{r^5}+B a^5\left(\frac{2Ex}{r^5}-\frac{5H x}{r^7}\right).
$$

At $r=a$, the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) requires $u'=-Ex$. Matching the independent $Ex$ and $Hx$ terms fixes $B=-1/2$ and $C=5/6$. The **disturbance velocity and pressure** are consequently

$$
\boxed{u'=-\frac{a^5}{r^5}Ex-\frac{5a^3}{2r^5}\left(1-\frac{a^2}{r^2}\right)H x,
\qquad p'=-\frac{5\mu a^3H}{r^5}.}
$$

The pressure follows from $p'=2\mu\nabla\cdot\Phi'$. The disturbance decays, the total velocity vanishes at the sphere, and the harmonic representation verifies the [Stokes equation](../../../../../stokes-equation.md). The boundary traction has zero total force by odd symmetry, and zero total torque because $E$ is symmetric, confirming the assumed [force-free](../../../../../force-free.md) and [torque-free](../../../../../torque-free.md) motion.

At the sphere $u'=-u_0$, so the [extra dissipation due to a rigid inclusion](../../../../../extra-dissipation-due-to-a-rigid-inclusion.md) becomes $\int_Au_0\cdot(\sigma_0+\sigma')N\,dS$. Contracting the supplied total [stress tensor](../../../../../cauchy-stress-tensor.md) with $N$ cancels its terms proportional to $(N\cdot EN)N$, leaving $5\mu EN$. Thus

$$
D'=5\mu a\int_A|EN|^2dS.
$$

Using $\int_AN_iN_jdS=4\pi a^2\delta_{ij}/3$ proves the **single-sphere dissipation increase**

$$
\boxed{D'=\frac{20\pi}{3}\mu a^3E:E.}
$$

One may perform the comparison in a large bounded vessel with prescribed straining velocity and then take its size to infinity; the given near-sphere approximation makes this limit compatible with the fixed-outer-velocity definition of $D'$.

The sphere number density is $n_s=\phi/(4\pi a^3/3)=3\phi/(4\pi a^3)$. Neglecting [hydrodynamic interactions](../../../../../hydrodynamic-interaction.md), the additional [viscous dissipation](../../../../../viscous-dissipation.md) per unit volume is $n_sD'=5\mu\phi E:E$. Adding the particle-free value $2\mu E:E$ gives

$$
2\mu_{\mathrm{eff}}E:E=2\mu E:E+5\mu\phi E:E,\qquad
\boxed{\mu_{\mathrm{eff}}=\mu\left(1+\frac52\phi\right).}
$$

This is the [Einstein viscosity formula for a dilute suspension](../../../../../einstein-viscosity-formula-for-a-dilute-suspension.md), to first order in the particle [volume fraction](../../../../../volume-fraction.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
