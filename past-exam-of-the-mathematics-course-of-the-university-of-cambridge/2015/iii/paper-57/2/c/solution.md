<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [MHD induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) can be written in material form as

$$
\frac{D\mathbf B}{Dt}
=(\mathbf B\cdot\nabla)\mathbf u-\mathbf B\,\nabla\cdot\mathbf u,
\qquad
\frac D{Dt}=\partial_t+u_x\partial_x+u_z\partial_z.
$$

Its $y$ component immediately gives

$$
\boxed{\frac{DB_y}{Dt}=\mathbf B\cdot\nabla u_y-B_y\nabla\cdot\mathbf u.}
$$

For the [Cartesian magnetic flux function](../../../../../../cartesian-magnetic-flux-function.md), the $x,z$ components of the [MHD induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md), or the $y$ component of the [magnetic vector potential](../../../../../../magnetic-vector-potential.md) equation, give

$$
\partial_t\psi+u_x\partial_x\psi+u_z\partial_z\psi=C(t).
$$

The additive function of time in $\psi$ has no effect on $\mathbf B$. Choose this gauge so that $C=0$. Then **the flux label is materially conserved**:

$$
\boxed{\frac{D\psi}{Dt}=0.}
$$

This is [magnetic flux freezing](../../../../../../magnetic-flux-freezing.md) in the two-dimensional geometry.

To prove the absence of axial motion, construct an invariant solution with $u_y=0$. Along each [Lagrangian trajectory](../../../../../../lagrangian-trajectory.md), $\psi$ is fixed, and the assumed divergence gives

$$
\frac{DB_y}{Dt}=-g(\psi,t)B_y,\qquad
B_y(\mathbf x,t)=
f(\psi(\mathbf x,t))
\exp\left[-\int_0^t g(\psi(\mathbf x,t),s)\,ds\right].
$$

Thus $B_y$ remains a function of $\psi$ and time alone. Its [gradient](../../../../../../gradient.md) stays parallel to $\nabla\psi$, so the $y$ component of the [Lorentz force](../../../../../../lorentz-force.md) remains zero. The axial momentum equation is

$$
\rho\frac{Du_y}{Dt}
=\frac1{\mu_0}(B_x\partial_x+B_z\partial_z)B_y=0,
$$

because $(B_x\partial_x+B_z\partial_z)\psi=0$. With $u_y=0$ initially, it remains zero. Hence **neither axial force nor axial motion is generated**. This [flux-surface preservation during magnetic-tube expansion](../../../../../../flux-surface-preservation-during-magnetic-tube-expansion.md) argument assumes the smooth ideal evolution for which the initial-value problem is unique; the particular in-plane rising motion need not be calculated.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
