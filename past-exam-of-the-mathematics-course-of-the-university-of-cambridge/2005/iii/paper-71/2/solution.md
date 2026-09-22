<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Linearizing the [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md) about a static [magnetic field](../../../../../magnetic-field.md) and using $u'=\partial_t\xi$ gives the [fluid Lagrangian displacement](../../../../../lagrangian-displacement-fluid-mechanics.md)-generated [magnetic field](../../../../../magnetic-field.md) perturbation $b=\nabla\times(\xi\times B)$. The two [solenoidal vector field](../../../../../solenoidal-vector-field.md) conditions reduce the [curl](../../../../../curl.md) identity to

$$
\boxed{b_i=B_j\partial_j\xi_i-\xi_j\partial_jB_i.}
$$

Its [divergence](../../../../../divergence.md) vanishes because it is a [curl](../../../../../curl.md). Directly, the two products of first derivatives in $\partial_ib_i$ cancel after exchanging their indices, while the remaining terms differentiate $\nabla\cdot\xi$ or $\nabla\cdot B$, both zero. Similarly the integrated linear [continuity equation](../../../../../continuity-equation.md) gives $\rho'=-\nabla\cdot(\rho\xi)$, so **$\boxed{\rho'=-\xi\cdot\nabla\rho}$**.

Let $\Pi=p+B^2/(2\mu_0)$ be the [magnetohydrodynamic total pressure](../../../../../magnetohydrodynamic-total-pressure.md). [Magnetostatic equilibrium](../../../../../magnetostatic-equilibrium.md) and the momentum equation in the [linearized ideal magnetohydrodynamic equations](../../../../../linearized-ideal-magnetohydrodynamic-equations.md) are

$$
\partial_i\Pi=-\rho\partial_i\Phi+\mu_0^{-1}B_j\partial_jB_i,
$$



$$
-\sigma^2\rho\xi_i=-\partial_i\pi'-\rho'\partial_i\Phi
+\mu_0^{-1}(B_j\partial_jb_i+b_j\partial_jB_i),\qquad
\pi'=p'+B\cdot b/\mu_0.
$$

There is no perturbed [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) here because the field is fixed. Multiply by $\xi_i^*$ and integrate. The [pressure](../../../../../pressure.md) term vanishes by the assumed boundary cancellation and $\nabla\cdot\xi^*=0$. Thus

$$
\sigma^2I=-\int\xi_i^*\xi_j\rho_{,j}\Phi_{,i}\,dV+\mu_0^{-1}\mathcal M,
\qquad I=\int\rho|\xi|^2dV,
$$

where $\mathcal M=-\int\xi_i^*(B_j\partial_jb_i+b_j\partial_jB_i)dV$.

Integrate the first magnetic term along $B$, using $\nabla\cdot B=0$, then insert the expression for $b$. This gives the positive term $\int|(B\cdot\nabla)\xi|^2dV$ and two mixed derivative terms. For clarity, the troublesome term transforms as

$$
-\int(B_k\partial_k\xi_i^*)\xi_j\partial_jB_i
=\int\xi_i^*B_k(\partial_k\xi_j)\partial_jB_i
+\int\xi_i^*\xi_jB_k\partial_k\partial_jB_i.
$$

The first term on the right cancels the other mixed term. Combining the remaining derivative with the term containing $\partial_jB_k\partial_kB_i$ gives

$$
\mathcal M=\int|(B\cdot\nabla)\xi|^2dV
+\int\xi_i^*\xi_j\partial_j(B_k\partial_kB_i)dV.
$$

Differentiating the equilibrium relation now combines the gradient of [mass density](../../../../../density.md) and [magnetostatic equilibrium](../../../../../magnetostatic-equilibrium.md) terms:

$$
-\rho_{,j}\Phi_{,i}+\mu_0^{-1}\partial_j(B_k\partial_kB_i)
=\Pi_{,ij}+\rho\Phi_{,ij}.
$$

We obtain the [incompressible magnetic displacement energy identity](../../../../../incompressible-magnetic-displacement-energy-identity.md)

$$
\boxed{\sigma^2I=\int\xi_i^*\xi_j\Pi_{,ij}dV
+\int\rho\xi_i^*\xi_j\Phi_{,ij}dV
+\frac1{\mu_0}\int|(B\cdot\nabla)\xi|^2dV.}
$$

The two [Hessian matrices](../../../../../hessian-matrix.md) are real symmetric, making their [Hermitian form](../../../../../hermitian-form.md) evaluations real. The last term is a squared [norm](../../../../../norm.md), and $I>0$ for a nonzero displacement in fluid with positive [mass density](../../../../../density.md). Thus **$\boxed{\sigma^2\text{ is real}}$**. It may be negative, in which case one temporal branch has exponential growth; real squared [frequency](../../../../../frequency.md) is not itself a proof of stability.

For the atmosphere with a horizontal [magnetic field](../../../../../magnetic-field.md), $\Phi=gz$ has zero [Hessian matrix](../../../../../hessian-matrix.md) and the equilibrium equation is

$$
\boxed{\frac{d}{dz}\left(p+\frac{B^2}{2\mu_0}\right)=-\rho g.}
$$

Consequently the [interchange stability of an incompressible magnetized atmosphere](../../../../../interchange-stability-of-an-incompressible-magnetized-atmosphere.md) is governed by the numerator

$$
Q[\xi]=-g\int\rho_z|\xi_z|^2dV+\frac1{\mu_0}\int B^2|\partial_x\xi|^2dV.
$$

For $\xi_z=\sin ky$, the [magnetic tension](../../../../../magnetic-tension.md) term is zero: these [fluid Lagrangian displacements](../../../../../lagrangian-displacement-fluid-mechanics.md) interchange neighboring [magnetic field lines](../../../../../magnetic-field-line.md) without varying along them. A [mass density](../../../../../density.md) increasing with height gives negative energy and instability; decreasing [mass density](../../../../../density.md) gives positive energy for these vertical interchanges. If $\rho_z\leq0$ everywhere, the displayed form is nonnegative for every admitted incompressible displacement. If the gradient changes sign, suitably localized [divergence](../../../../../divergence.md)-free interchange trials detect an unstable inverted layer; For example, take $\xi_z=f(z)e^{iky}$ and $\xi_y=if'(z)e^{iky}/k$, with $f$ supported in that layer. Their [divergence](../../../../../divergence.md) is zero, and neither component varies along the [magnetic field](../../../../../magnetic-field.md).

For $\xi_z=\sin kx$, [magnetic field lines](../../../../../magnetic-field-line.md) are bent. Averaging over a full horizontal [wavelength](../../../../../wavelength.md) gives the trial [Rayleigh quotient](../../../../../rayleigh-quotient.md)

$$
\frac{Q}{I}=\frac{-g\int\rho_z\,dz+(k^2/\mu_0)\int B^2\,dz}{\int\rho\,dz},
$$

under the stipulated admissible boundary/integrability conditions. It is a trial quotient, not a claim that this displacement is an exact [eigenfunction](../../../../../eigenfunction.md) for every profile. [mass density](../../../../../density.md) decreasing upward is stable here too. For inverted [mass density](../../../../../density.md), [magnetic tension](../../../../../magnetic-tension.md) can stabilize sufficiently short waves along the [magnetic field](../../../../../magnetic-field.md), but does not remove the transverse interchange instability. Locally the two contributions have the familiar scale $-g\rho_z/\rho+k^2v_A^2$, with the [Alfvén speed](../../../../../alfven-speed.md) $v_A=B/\sqrt{\mu_0\rho}$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
