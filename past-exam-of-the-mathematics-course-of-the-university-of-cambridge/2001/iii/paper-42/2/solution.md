<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [magnetohydrodynamic total pressure](../../../../../magnetohydrodynamic-total-pressure.md) is

$$
\boxed{\Pi=p+\frac{B^2}{2\mu_0}.}
$$

The [Lorentz force](../../../../../lorentz-force.md) has been split into the [gradient](../../../../../gradient.md) of [magnetic pressure](../../../../../magnetic-pressure.md) and the remaining [magnetic tension](../../../../../magnetic-tension.md) term. An appropriate boundary model is impermeable, perfectly conducting stationary cylindrical walls with no initial normal [magnetic flux](../../../../../magnetic-flux.md): $u_r=B_r=0$ at $r=a,b$. In an inviscid fluid this is a slip condition, not a no-slip condition on $u_\phi$ or $u_z$. It also makes the tangential ideal [electric field](../../../../../electric-field.md) vanish at the walls. Take [perturbations](../../../../../perturbation.md) periodic in $\phi$ and periodic or Fourier-resolved in $z$; the wall reaction supplies the normal [pressure](../../../../../pressure.md) force without an extra prescribed [pressure](../../../../../pressure.md) value.

Write the steady [velocity](../../../../../velocity.md) and [magnetic field](../../../../../magnetic-field.md) as $U(r)\mathbf e_\phi$ and $B(r)\mathbf e_\phi$. They satisfy both [divergence](../../../../../divergence.md) constraints. Their material accelerations have only radial curvature terms, and the steady [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md) is identically satisfied because the parallel azimuthal flow and field have cancelling curvature terms. The radial momentum equation is

$$
-\rho\frac{U^2}r=-\frac{d\Pi}{dr}-\frac{B^2}{\mu_0r}.
$$

Hence the most general such equilibrium is

$$
\boxed{U(r),B(r)\text{ arbitrary smooth functions},\qquad
\Pi(r)=\Pi_0+\int_{r_0}^r\left(\frac{\rho U(s)^2}s-\frac{B(s)^2}{\mu_0s}\right)ds.}
$$

Its [gas pressure](../../../../../gas-pressure.md) is $p=\Pi-B^2/(2\mu_0)$; on a bounded annulus the additive constant can be chosen to keep it positive. Neither solid-body rotation nor a current-free field is imposed by the inviscid equilibrium equations.

For the [linear stability](../../../../../linear-stability.md) calculation, put $\Omega=U/r$, $V=B/\sqrt{\mu_0\rho}$, and define $h=\delta\Pi/\rho$. Use axisymmetric [normal modes](../../../../../normal-mode.md) proportional to $e^{ikz-i\omega t}$. Denote the [velocity](../../../../../velocity.md) amplitudes by $(u,v,w)$ and the magnetic amplitudes in [velocity](../../../../../velocity.md) units by $(b_r,b_\phi,b_z)=\delta\mathbf B/\sqrt{\mu_0\rho}$. [Linearization](../../../../../linearization.md) of the cylindrical momentum equations gives

$$
\begin{aligned}
-i\omega u-2\Omega v&=-h'-\frac{2V}r b_\phi,\\
-i\omega v+(2\Omega+r\Omega')u&=(V'+V/r)b_r,\\
-i\omega w&=-ikh.
\end{aligned}
$$

The linearized [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md) and [divergence](../../../../../divergence.md) equations are

$$
\begin{aligned}
-i\omega b_r&=0,\\
-i\omega b_\phi&=r\Omega'b_r+(V/r-V')u,\\
-i\omega b_z&=0,\\
\frac{(ru)'}r+ikw&=0,\qquad
\frac{(rb_r)'}r+ikb_z=0.
\end{aligned}
$$

The curvature terms are essential: although the [perturbations](../../../../../perturbation.md) have no azimuthal dependence, the cylindrical unit vectors do.

For $\omega\ne0$, $b_r=b_z=0$. Introduce the radial [Lagrangian fluid displacement](../../../../../lagrangian-fluid-displacement.md) by $u=-i\omega\xi$. The azimuthal amplitudes reduce to

$$
v=-(2\Omega+r\Omega')\xi,\qquad
b_\phi=(V/r-V')\xi.
$$

Consequently the radial and vertical equations, combined with the [incompressible flow](../../../../../incompressible-flow.md) constraint, give

$$
h'=(\omega^2-\mathcal D)\xi,\qquad
h=\frac{\omega^2}{k^2}\frac{(r\xi)'}r,
$$

where the [Michael criterion for axisymmetric toroidal-field interchange](../../../../../michael-criterion-for-axisymmetric-toroidal-field-interchange.md) coefficient is

$$
\boxed{\mathcal D(r)=\kappa^2-r\frac{d}{dr}\left(\frac{V^2}{r^2}\right),\qquad
\kappa^2=4\Omega^2+2r\Omega\Omega'.}
$$

For $k\ne0$, the required single displacement equation is therefore

$$
\boxed{\omega^2\left[-\frac{d}{dr}\left(\frac{(r\xi)'}r\right)+k^2\xi\right]
=k^2\mathcal D\xi,\qquad \xi(a)=\xi(b)=0.}
$$

The same differential equation holds for $u$, which is a constant multiple of $\xi$.

Set $y=r\xi$. Multiplication by $y^*$ and [integration by parts](../../../../../integration-by-parts.md) with the wall conditions gives the [global variational form of the Michael criterion](../../../../../global-variational-form-of-the-michael-criterion.md):

$$
\boxed{\omega^2=k^2\frac{\displaystyle\int_a^b\mathcal D\,|y|^2/r\,dr}
{\displaystyle\int_a^b(|y'|^2+k^2|y|^2)/r\,dr}.}
$$

The denominator is strictly positive for a nonzero displacement, so every mode's $\omega^2$ is real. If $\mathcal D\geq0$ everywhere, no exponentially growing mode exists. Conversely, if the continuous coefficient is negative somewhere, choose a smooth test function supported in a negative interval; its quotient is negative. For sufficiency, let $A=-d(r^{-1}d/dr)/dr+k^2/r$ be the positive [Sturm-Liouville operator](../../../../../sturm-liouville-operator.md) with [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) and let $C$ multiply by $k^2\mathcal D/r$. The generalized mode equation $\omega^2Ay=Cy$ is equivalent to the [compact operator](../../../../../compact-operator-split.md) and [self-adjoint operator](../../../../../self-adjoint-operator.md) problem $A^{-1/2}CA^{-1/2}f=\omega^2f$. The negative test quotient guarantees a negative [eigenvalue](../../../../../eigenvalue.md) and therefore a growing solution $\omega=i\gamma$. This argument remains valid when the coefficient changes sign, without incorrectly assuming a positive weight in [Sturm-Liouville theory](../../../../../sturm-liouville-theory.md).

Thus, for any fixed nonzero vertical [wavenumber](../../../../../wavenumber.md),

$$
\boxed{\text{axisymmetric exponential instability}\quad\Longleftrightarrow\quad
\kappa^2-r\frac{d}{dr}\left(\frac{B_\phi^2}{\mu_0\rho r^2}\right)<0\ \text{somewhere}.}
$$

Equality is marginal. When $k=0$, the [incompressible flow](../../../../../incompressible-flow.md) constraint and both rigid-wall conditions force the radial [velocity](../../../../../velocity.md) to vanish, so that special case has no radial interchange mode. When the field vanishes, the coefficient reduces to $\kappa^2=r^{-3}(r^4\Omega^2)'$, recovering the [Rayleigh centrifugal stability criterion](../../../../../rayleigh-centrifugal-stability-criterion.md).

For a [Keplerian disk](../../../../../keplerian-disk.md), $\kappa^2=\Omega^2$. If $B_\phi\propto r^p$, the [toroidal interchange field threshold in a thin Keplerian disk](../../../../../toroidal-interchange-field-threshold-in-a-thin-keplerian-disk.md) is

$$
\mathcal D=\Omega^2-2(p-1)V^2/r^2<0,
\qquad\boxed{p>1,\quad V^2>\frac{r^2\Omega^2}{2(p-1)}.}
$$

For ordinary radial gradients on the scale $r$, the [Alfvén speed](../../../../../alfven-speed.md) must therefore be comparable to the orbital speed. A field on the [gas pressure](../../../../../gas-pressure.md) scale has $V\lesssim c_s\sim H\Omega\ll r\Omega$ in a [thin disk](../../../../../thin-disk.md), and cannot normally meet this condition. Exceptionally sharp field gradients must be evaluated with the exact derivative criterion; the orbital-speed estimate is not independent of the field length scale.

This is a toroidal magnetic interchange driven by the field/current distribution, opposed by restoration set by the [radial epicyclic frequency](../../../../../radial-epicyclic-frequency.md). It is **not the usual weak vertical-field [magnetorotational instability](../../../../../magnetorotational-instability.md)**. In the vertical-field problem, a nonzero $kB_z$ bends [magnetic field lines](../../../../../magnetic-field-line.md) and couples displaced fluid elements, allowing decreasing $\Omega$ to supply [rotational kinetic energy](../../../../../rotational-kinetic-energy.md) even when $\kappa^2>0$. Here the axisymmetric [perturbation](../../../../../perturbation.md) has no scalar variation along the purely toroidal background field, and no such weak-field coupling: a sufficiently adverse toroidal-field gradient, rather than merely $d\Omega/dr<0$, is required. Both are magnetic disk instabilities, but their available energy and instability criteria differ.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
