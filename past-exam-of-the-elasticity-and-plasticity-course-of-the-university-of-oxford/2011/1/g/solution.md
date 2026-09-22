<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The multiplier enforcing [elastic incompressibility](../../../../elastic-incompressibility.md) contributes an arbitrary hydrostatic [stress](../../../../stress.md). Denote it by $q(r)$ to distinguish it from the applied [pressure](../../../../pressure-split.md) $P$. For the [neo-Hookean solid](../../../../neo-hookean-solid.md), the [Cauchy stress tensor](../../../../cauchy-stress-tensor.md) is $\tau=-qI+\mu FF^T$. Thus its principal components are

$$
\boxed{t_r=-q+\mu\lambda_r^2=-q+\mu\frac{R^2}{r^2},\qquad
t_\theta=-q+\mu\lambda_\theta^2=-q+\mu\frac{r^2}{R^2}.}
$$

The axial component is $t_z=-q+\mu$, despite the unit axial stretch. The quantity $q$ is a [Lagrange multiplier](../../../../lagrange-multiplier.md) determined together with equilibrium and the [traction](../../../../traction.md) conditions; it is not obtained by differentiating the reduced stretch [energy](../../../../energy-split.md) while ignoring its constraint.

In particular the [stress](../../../../stress.md) difference eliminates this multiplier:

$$
\boxed{t_\theta-t_r=\mu\left(\frac{r^2}{R^2}-\frac{R^2}{r^2}\right).}
$$

## ↑ Ancestors (12)

1. [G](../g.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
