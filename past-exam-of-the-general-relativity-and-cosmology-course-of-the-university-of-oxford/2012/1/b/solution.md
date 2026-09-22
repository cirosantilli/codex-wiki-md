<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [curvature sign convention](../../../../curvature-sign-convention.md)

$$
R^\rho{}_{\sigma\mu\nu}=\partial_\mu\Gamma^\rho{}_{\nu\sigma}-\partial_\nu\Gamma^\rho{}_{\mu\sigma}+\Gamma^\rho{}_{\mu\lambda}\Gamma^\lambda{}_{\nu\sigma}-\Gamma^\rho{}_{\nu\lambda}\Gamma^\lambda{}_{\mu\sigma},
$$

which has the derivative ordering printed in the source for $R^i{}_{0j0}$. A [Christoffel symbol](../../../../christoffel-symbol.md) is of order $\mu/r^2$, so its derivative is of order $\mu/r^3$, whereas a product of two connections is of order $\mu^2/r^4$. Their ratio is $\mu/r\ll1$. The metric is stationary, hence the temporal derivative term vanishes. Consequently

$$
R^i{}_{0j0}\simeq\partial_j\Gamma^i{}_{00}=-\frac12\partial_i\partial_jg_{00}.
$$

Here $g_{00}=-1+2\mu/r$, and $\partial_i\partial_j(1/r)=(3x_ix_j-r^2\delta_{ij})/r^5$. The [weak-field tidal curvature in a stationary metric](../../../../weak-field-tidal-curvature-in-a-stationary-metric.md) is

$$
\boxed{R^i{}_{0j0}=\frac{GM}{c^2r^3}\left(\delta_{ij}-3\frac{x^ix^j}{r^2}\right)+O(\mu^2/r^4).}
$$

**Printed sign inconsistency.** The source's positive half-Hessian and its final negative-prefactor expression are the opposites of this result. A concrete check at $(r,0,0)$ is $\Gamma^1{}_{00}\simeq\mu/r^2$, giving $\partial_1\Gamma^1{}_{00}=-2\mu/r^3$, while the printed final expression gives $+2\mu/r^3$. Thus both printed equalities cannot hold with its stated derivative ordering. Reversing the definition of the [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md) would give the printed final sign, but would also require reversing the curvature term in the [geodesic deviation](../../../../geodesic-deviation.md) equation. The convention used here and in the next part gives the physical radial stretching and transverse compression.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
