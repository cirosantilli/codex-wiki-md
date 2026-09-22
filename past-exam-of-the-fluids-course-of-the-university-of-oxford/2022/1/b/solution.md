<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a fixed representative volume $V$ containing many pores. Let $\varphi$ be the [porosity](../../../../porosity.md) and let $\mathbf q$ be the [Darcy velocity](../../../../darcy-velocity.md), defined per unit total area. The [conservation of mass](../../../../mass-conservation.md) is

$$
\frac{d}{dt}\int_V\varphi\rho\,dV
=-\int_{\partial V}\rho\mathbf q\cdot\mathbf n\,dS.
$$

The solid matrix is rigid and fixed, and the liquid is fully saturating and has constant [mass density](../../../../density.md), so the stored mass on the left is constant. Microscopic internal liquid-solid boundaries contribute no through-flux by the [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md). Applying the [divergence theorem](../../../../divergence-theorem.md) to the external flux gives

$$
\int_V\nabla\cdot(\rho\mathbf q)\,dV=0.
$$

Since the representative volume is arbitrary, the macroscopic [continuity equation](../../../../continuity-equation.md) is

$$
\boxed{\nabla\cdot(\rho\mathbf q)=0,\qquad \nabla\cdot\mathbf q=0\quad\text{for constant }\rho.}
$$

There is no extra factor of $\varphi$ in the flux: that factor is already incorporated in the definition of the [Darcy velocity](../../../../darcy-velocity.md). A compressible liquid or deformable matrix would require retaining the storage term.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
