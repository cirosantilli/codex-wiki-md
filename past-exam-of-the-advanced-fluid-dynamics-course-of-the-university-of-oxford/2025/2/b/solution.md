<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For two [Stokes flows](../../../../stokes-flow-split.md) in the same fluid domain with the same [dynamic viscosity](../../../../dynamic-viscosity-split.md), symmetry of the [Newtonian fluid stress tensor](../../../../newtonian-fluid-stress-tensor.md) and [incompressibility](../../../../incompressible-flow.md) give the local reciprocal identity

$$
\nabla\cdot(\boldsymbol\sigma\mathbf u'-\boldsymbol\sigma'\mathbf u)=0.
$$

In [index notation](../../../../index-notation.md), its remaining cross-gradient terms are both $2\mu e:e'$. On the remote sphere the integrated reciprocal flux tends to zero: the [velocity](../../../../velocity.md) is $O(R^{-1})$, the [stress tensor](../../../../cauchy-stress-tensor.md) is $O(R^{-2})$ and the area is $O(R^2)$. On the body, the [no-slip boundary condition](../../../../no-slip-boundary-condition.md) makes the two [velocities](../../../../velocity.md) the constants $\mathbf U,\mathbf U'$. The [Lorentz reciprocal theorem](../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) therefore gives

$$
\boxed{\mathbf F\cdot\mathbf U'=\mathbf F'\cdot\mathbf U.}
$$

By the [Linearity of Stokes flow](../../../../linearity-of-stokes-flow.md), the sum of the two velocity-pressure fields satisfies the boundary conditions for body [velocity](../../../../velocity.md) $\mathbf U+\mathbf U'$. Uniqueness of the exterior [Stokes flow](../../../../stokes-flow-split.md) identifies it with the third solution. Since the [stress tensor](../../../../cauchy-stress-tensor.md) and its surface [integral](../../../../integral-split.md) are linear too, $\mathbf F(\mathbf U+\mathbf U')=\mathbf F(\mathbf U)+\mathbf F(\mathbf U')$; scalar multiplication follows in the same way. Thus $\mathbf F=-A\mathbf U$ for a fixed-orientation [hydrodynamic resistance matrix](../../../../hydrodynamic-resistance-matrix.md) $A$. Substituting arbitrary $\mathbf U,\mathbf U'$ in the reciprocal identity yields

$$
\boxed{A=A^T,\qquad\mathbf F=-A\mathbf U.}
$$

The minus sign is natural because [viscous dissipation](../../../../viscous-dissipation.md) gives $-\mathbf F\cdot\mathbf U=2\mu\int e:e\,dV>0$ for nonzero rigid translation in an otherwise stationary fluid; $A$ is a [positive-definite matrix](../../../../positive-definite-matrix.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
