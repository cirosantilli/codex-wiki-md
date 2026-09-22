<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [stress tensor](../../../../cauchy-stress-tensor.md) of the incompressible [Newtonian fluid](../../../../newtonian-fluid.md) is $\boldsymbol\sigma=-pI+2\mu e$, where $e=(\nabla\mathbf u+\nabla\mathbf u^T)/2$ is the [rate-of-strain tensor](../../../../strain-rate-tensor.md). The homogeneous [Stokes equations](../../../../stokes-equation.md) give $\nabla\cdot\boldsymbol\sigma=0$. Apply the [divergence theorem](../../../../divergence-theorem.md) to the fluid between the body and a surrounding sphere $S_R$. If $\mathbf n_B$ points from the body into the fluid, the fluid-domain normal on the inner boundary is $-\mathbf n_B$. Hence

$$
0=\int_{S_R}\boldsymbol\sigma\mathbf n\,dS-\int_{\partial B}\boldsymbol\sigma\mathbf n_B\,dS,
\qquad\boxed{\mathbf F=\int_{S_R}\boldsymbol\sigma\mathbf n\,dS.}
$$

This is the [force flux at infinity in Stokes flow](../../../../force-flux-at-infinity-in-stokes-flow.md). A nonzero resultant [force](../../../../force-split.md) must be supported by a stress of order $R^{-2}$ on a surface of area of order $R^2$. More precisely, the leading exterior solution is a [Stokeslet](../../../../stokeslet.md) with force on the fluid $\mathbf f=-\mathbf F$:

$$
\mathbf u(\mathbf x)\sim\frac{(I+\widehat{\mathbf x}\widehat{\mathbf x}^{T})\mathbf f}{8\pi\mu R},\qquad
p(\mathbf x)-p_\infty\sim\frac{\mathbf f\cdot\widehat{\mathbf x}}{4\pi R^2}.
$$

Thus $\mathbf u=O(R^{-1})$, $p-p_\infty=O(R^{-2})$ and $e=O(R^{-2})$. These are leading generic orders for a translating body with nonzero drag; the integral alone does not determine every angular component, and force-free disturbances may decay faster.

## ↑ Ancestors (12)

1. [A](../a.md)
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
