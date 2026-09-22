<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $u=psi_z$ and $w=-psi_x$, so [mass conservation](../../../../../../mass-conservation.md) for the two-dimensional [incompressible flow](../../../../../../incompressible-flow.md) is automatic. Write $b$ for buoyancy and introduce the diffusive operators

$$
D_\nu=\partial_t-\nu\nabla^2,
\qquad
D_\kappa=\partial_t-\kappa\nabla^2.
$$

The [Linearized Boussinesq equations](../../../../../../linearized-boussinesq-equations.md) are

$$
D_\nu u=-\frac1{\rho_0}p_x,
\qquad
D_\nu w=-\frac1{\rho_0}p_z+b,
\qquad
D_\kappa b=-N^2w.
$$

Taking the curl of the [momentum conservation](../../../../../../momentum-conservation.md) equations eliminates the [pressure](../../../../../../pressure.md) and gives

$$
-D_\nu\nabla^2\psi=b_x.
$$

Apply $D_\kappa$ and use $D_\kappa b=N^2\psi_x$. Since the constant-coefficient [linear partial differential operators](../../../../../../linear-partial-differential-operator.md) commute,

$$
\boxed{\left[D_\nu D_\kappa\nabla^2+N^2\partial_x^2\right]\psi=0.}
$$

This is the viscous-diffusive [internal gravity wave](../../../../../../internal-wave.md) equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
