<h1 id="1/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

The radial equilibrium equation gives $dt_r/dr=(t_\theta-t_r)/r$. Set $C=a^2-A^2$, so that $R^2=r^2-C$. Substitution of the [neo-Hookean solid](../../../../neo-hookean-solid.md) [stress](../../../../stress.md) difference eliminates both $q$ and $t_\theta$:

$$
\boxed{\frac{dt_r}{dr}=\frac\mu r\left[\frac{r^2}{r^2-C}-\frac{r^2-C}{r^2}\right]
=\frac{\mu C(2r^2-C)}{r^3(r^2-C)},\qquad a<r<b.}
$$

This is a first-order [ordinary differential equation](../../../../ordinary-differential-equation.md) for the radial [stress](../../../../stress.md), parametrized by the unknown inner radius. For inflation $C>0$, its right side is positive, so $t_r$ increases from the negative inner [pressure](../../../../pressure-split.md) to zero at the outer surface. The denominator stays positive because $r^2-C=R^2\geq A^2>0$.

## ↑ Ancestors (12)

1. [H](../h.md)
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
