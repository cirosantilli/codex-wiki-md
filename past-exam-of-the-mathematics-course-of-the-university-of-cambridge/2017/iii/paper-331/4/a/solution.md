<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $\nu=Re^{-1}>0$, $\kappa=Pe^{-1}>0$, $\mathbf U=\overline{\mathbf u}+\mathbf u$, and $\Theta=\overline\theta+\theta$. Work along a sufficiently regular direct trajectory satisfying the given constraints. The zero spatial mean of the [scalar field](../../../../../../scalar-field.md) is conserved by [incompressible flow](../../../../../../incompressible-flow.md), impermeable walls and zero scalar flux, so minimizing $J=(\Theta(T),\Theta(T))$ is equivalent to minimizing [scalar variance](../../../../../../scalar-variance.md), up to the fixed domain volume.

The printed functional fixes the initial state to a candidate $\mathbf u_0$; it contains no term that enforces its [kinetic energy](../../../../../../kinetic-energy.md). For the optimization over that candidate, add the real [Lagrange multiplier](../../../../../../lagrange-multiplier.md) constraint

$$
\mathcal L_E=\mathcal L-\lambda\left[\frac12(\mathbf u_0,\mathbf u_0)-E_0\right].
$$

Equivalently, one can restrict all control variations to the [sphere in a normed vector space](../../../../../../sphere-in-a-normed-vector-space.md) of fixed [kinetic energy](../../../../../../kinetic-energy.md). This term changes the initial-control optimality condition, not the interior adjoint equations.

Let $\mathbf v=\delta\mathbf u$, $\sigma=\delta\theta$ and $\pi=\delta p$. [Linearization](../../../../../../linearization.md) of the momentum and [scalar transport](../../../../../../scalar-transport.md) residuals gives

$$
\delta F_u=\partial_t\mathbf v+\mathbf U\cdot\nabla\mathbf v
+\mathbf v\cdot\nabla\mathbf U+Ri_B\sigma\hat{\mathbf y}
+\nabla\pi-\nu\Delta\mathbf v,
$$



$$
\delta F_\theta=\partial_t\sigma+\mathbf U\cdot\nabla\sigma
+\mathbf v\cdot\nabla\Theta-\kappa\Delta\sigma.
$$

Both appearances of the perturbation [velocity](../../../../../../velocity.md) in the nonlinear momentum term have been differentiated. In particular, the coefficient is the [gradient](../../../../../../gradient.md) of the total [velocity](../../../../../../velocity.md), not just the base shear.

For the negative-constraint convention of the functional, [integration by parts](../../../../../../integration-by-parts.md) gives the interior coefficients of $\mathbf v,\sigma,\pi$ as

$$
\begin{aligned}
A_u&=\partial_t\mathbf u^\dagger+\mathbf U\cdot\nabla\mathbf u^\dagger
-(\nabla\mathbf U)^T\mathbf u^\dagger+\nabla p^\dagger
+\nu\Delta\mathbf u^\dagger-\theta^\dagger\nabla\Theta,\\
A_\theta&=\partial_t\theta^\dagger+\mathbf U\cdot\nabla\theta^\dagger
+\kappa\Delta\theta^\dagger-Ri_Bu_y^\dagger,\\
A_p&=\nabla\cdot\mathbf u^\dagger.
\end{aligned}
$$

Thus the [adjoint equations for Boussinesq scalar mixing](../../../../../../adjoint-equations-for-boussinesq-scalar-mixing.md) are

$$
\boxed{A_u=0,\qquad A_\theta=0,\qquad \nabla\cdot\mathbf u^\dagger=0.}
$$

The transpose is essential: the $j$th component of $(\nabla\mathbf U)^T\mathbf u^\dagger$ is $\sum_i u_i^\dagger\partial_jU_i$. The coupling $-\theta^\dagger\nabla\Theta$ transposes advection of the scalar by a [velocity](../../../../../../velocity.md) perturbation; $-Ri_Bu_y^\dagger$ transposes [buoyancy](../../../../../../buoyancy.md) feedback. Dropping the latter would give a [passive scalar](../../../../../../passive-scalar.md) adjoint, not the [active scalar](../../../../../../active-scalar.md) problem.

These equations are integrated backward, not forward. If $\tau=T-t$, they read

$$
\partial_\tau\mathbf u^\dagger=\mathbf U\cdot\nabla\mathbf u^\dagger
-(\nabla\mathbf U)^T\mathbf u^\dagger+\nabla p^\dagger
+\nu\Delta\mathbf u^\dagger-\theta^\dagger\nabla\Theta,
$$



$$
\partial_\tau\theta^\dagger=\mathbf U\cdot\nabla\theta^\dagger
+\kappa\Delta\theta^\dagger-Ri_Bu_y^\dagger,
$$

with direct coefficients evaluated at $t=T-\tau$. Both terms from the [diffusion equation](../../../../../../diffusion-equation-split.md) now have the usual forward sign in $\tau$. A [direct-adjoint looping](../../../../../../direct-adjoint-looping.md) method stores or reconstructs the forward trajectory, solves these equations backward, and uses the initial adjoint as the control [gradient](../../../../../../gradient.md). The endpoint and fixed-energy conditions below give necessary conditions for a local optimizer, not a global optimality theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
