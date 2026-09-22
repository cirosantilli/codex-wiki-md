# Adjoint equations for Boussinesq scalar mixing

↑ **Parent:** [Scalar transport](scalar-transport.md)

For a smooth incompressible direct trajectory with total [velocity field](velocity-field.md) $\mathbf U$ and [active scalar](active-scalar.md) $\Theta$, the negative-constraint [Lagrangian function in constrained optimization](lagrangian-function-in-constrained-optimization.md) convention gives

$$
\partial_t\mathbf u^\dagger+\mathbf U\cdot\nabla\mathbf u^\dagger-(\nabla\mathbf U)^T\mathbf u^\dagger+\nabla p^\dagger+\nu\Delta\mathbf u^\dagger-\theta^\dagger\nabla\Theta=0,\qquad \nabla\cdot\mathbf u^\dagger=0,
$$



$$
\partial_t\theta^\dagger+\mathbf U\cdot\nabla\theta^\dagger+\kappa\Delta\theta^\dagger-\mathrm{Ri}_B u_y^\dagger=0.
$$

The transpose term is the [formal adjoint](formal-adjoint.md) of $\delta\mathbf u\cdot\nabla\mathbf U$; the two couplings transpose [scalar transport](scalar-transport.md) by [advection](advection.md) and [buoyancy](buoyancy.md). For terminal cost $\int\Theta(T)^2$, the terminal data are $\mathbf u^\dagger(T)=0$, $\theta^\dagger(T)=2\Theta(T)$. They are integrated backward along the stored direct trajectory. [No-slip boundary conditions](no-slip-boundary-condition.md) and [Dirichlet boundary conditions](dirichlet-boundary-condition.md) for the adjoint [velocity](velocity.md) and homogeneous [Neumann boundary conditions](neumann-boundary-condition.md) for the adjoint scalar remove the spatial boundary terms.

## ↑ Ancestors (5)

1. [Scalar transport](scalar-transport.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Active scalar](active-scalar.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-331/4/a/solution.md)
