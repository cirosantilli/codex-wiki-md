<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For an [incompressible flow](../../../../../incompressible-flow.md), write the [Newtonian fluid stress tensor](../../../../../newtonian-fluid-stress-tensor.md) as $\sigma=-pI+2\mu e$, where $e=(\nabla u+\nabla u^T)/2$ is the [rate-of-strain tensor](../../../../../strain-rate-tensor.md). The [Stokes equation](../../../../../stokes-equation.md) gives $\partial_j\sigma_{ij}=0$. Symmetry of the [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) therefore gives

$$
\partial_j(u_i\sigma_{ij})=\sigma_{ij}\partial_j u_i=\sigma:e=2\mu e:e.
$$

Integrating and applying the [divergence theorem](../../../../../divergence-theorem.md) expresses the [viscous dissipation](../../../../../viscous-dissipation.md) as boundary power:

$$
\boxed{D=\int_{\partial V}u\cdot\sigma n\,dS.}
$$

At a moving [rigid body](../../../../../rigid-body-dynamics.md), the surface [velocity](../../../../../velocity.md) is $U+\Omega\times(x-x_c)$. Its boundary-power contribution is $U\cdot F+\Omega\cdot G$, with the [force](../../../../../force.md) and [torque](../../../../../torque.md) evaluated using the fluid's outward [normal vector](../../../../../normal-vector.md). Both resultants vanish for a [force-free](../../../../../force-free.md), [torque-free](../../../../../torque-free.md) inclusion. Thus the new [viscous dissipation](../../../../../viscous-dissipation.md) comes entirely from the unchanged outer boundary [velocity](../../../../../velocity.md). Subtracting the particle-free boundary power gives

$$
D'=\int_{\partial V_0}U_0\cdot\sigma'n\,dS.
$$

Apply the [Lorentz reciprocal theorem](../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) to $(u_0,\sigma_0)$ and $(u',\sigma')$ in the fluid outside the inclusion. On the outer boundary $u'=0$, so

$$
0=D'+\int_A(u_0\cdot\sigma'-u'\cdot\sigma_0)n\,dS.
$$

Writing $n_p=-n$ for the particle's outward [normal vector](../../../../../normal-vector.md) gives the required [extra dissipation due to a rigid inclusion](../../../../../extra-dissipation-due-to-a-rigid-inclusion.md):

$$
\boxed{D'=\int_A(u_0\cdot\sigma'-u'\cdot\sigma_0)n_p\,dS.}
$$

This subtraction already accounts for the fluid volume displaced by the inclusion; it is not just the integral of the disturbance's local [viscous dissipation](../../../../../viscous-dissipation.md).

For the sphere, the ambient [rate-of-strain tensor](../../../../../strain-rate-tensor.md) $E$ is symmetric and trace free. The [sphere in a uniform straining Stokes flow](../../../../../sphere-in-a-uniform-straining-stokes-flow.md) has zero translational and rotational [velocity](../../../../../velocity.md): inversion symmetry eliminates its [force](../../../../../force.md), and symmetry of $E$ eliminates its [torque](../../../../../torque.md). To derive the disturbance, put $r=|x|$, $Q=x\cdot Ex$ and seek

$$
u'=f(r)Ex+g(r)Qx,\qquad p'=\mu j(r)Q.
$$

The [incompressible flow](../../../../../incompressible-flow.md) condition and [Stokes equation](../../../../../stokes-equation.md) reduce to

$$
\frac{f'}r+rg'+5g=0,\qquad
f''+\frac4r f'+4g=2j,\qquad
g''+\frac8r g'=\frac{j'}r.
$$

A decaying family satisfying these equations is $f=Ar^{-5}$, $g=Br^{-5}-5Ar^{-7}/2$, $j=2Br^{-5}$. The [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) requires $f(a)=-1$ and $g(a)=0$, so $A=-a^5$ and $B=-5a^3/2$. Consequently

$$
\boxed{u'=-\frac{a^5}{r^5}Ex-\frac{5a^3}{2r^5}\left(1-\frac{a^2}{r^2}\right)(x\cdot Ex)x,\qquad
p'=-\frac{5\mu a^3}{r^5}(x\cdot Ex).}
$$

The total [velocity](../../../../../velocity.md) is zero at $r=a$, and the disturbance decays as $r^{-2}$. The pressure constant has been set to zero. These boundary and far-field conditions, together with [Uniqueness of Stokes flow](../../../../../uniqueness-of-stokes-flow.md), establish the solution. There is no rotational background in a pure strain flow.

On the sphere $u'=-u_0=-aEn_p$. Contracting the supplied [Newtonian fluid stress tensor](../../../../../newtonian-fluid-stress-tensor.md) with $n_p$ makes its two terms proportional to $(n_p\cdot En_p)n_p$ cancel, leaving $\sigma n_p=5\mu En_p$. Hence the [extra dissipation due to a rigid inclusion](../../../../../extra-dissipation-due-to-a-rigid-inclusion.md) is

$$
D'=5\mu a\int_A|En_p|^2\,dS
=5\mu a^3 E_{ij}E_{ik}\frac{4\pi}{3}\delta_{jk}
=\boxed{\frac{20\pi}{3}\mu a^3 E:E}.
$$

Here $\int_{S^2}n_jn_k\,d\Omega=4\pi\delta_{jk}/3$. Taking the large outer boundary limit only after using the fixed-boundary power identity avoids replacing that prescribed boundary by an uncontrolled boundary at infinity.

If $N_v$ denotes the number of spheres per unit volume, $N_v(4\pi a^3/3)=\phi$. Thus

$$
\boxed{N_v=\frac{3\phi}{4\pi a^3},\qquad N_vD'=5\mu\phi E:E.}
$$

Add this to the particle-free [viscous dissipation](../../../../../viscous-dissipation.md) density $2\mu E:E$. Comparing with $2\mu_{\mathrm{eff}}E:E$ gives the [Einstein viscosity formula for a dilute suspension](../../../../../einstein-viscosity-formula-for-a-dilute-suspension.md):

$$
\boxed{\mu_{\mathrm{eff}}=\mu\left(1+\frac52\phi\right)}
$$

to first order in $\phi$. The [hydrodynamic interactions](../../../../../hydrodynamic-interaction.md) neglected here contribute beyond that dilute order.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
