<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $\rho$ for the [mass density](../../../../../density.md). A material [volume](../../../../../volume.md) contains the same [fluid elements](../../../../../fluid-element.md) at all times, so [conservation of mass](../../../../../mass-conservation.md) requires

$$
0=\frac d{dt}\int_{V(t)}\rho\,dV=\int_{V(t)}\left(\partial_t\rho+\nabla\cdot(\rho\mathbf u)\right)dV,
$$

by the [Reynolds transport theorem](../../../../../reynolds-transport-theorem.md). Since the initial material [volume](../../../../../volume.md) can be chosen arbitrarily, continuity of the integrand forces it to vanish pointwise. Thus the [continuity equation](../../../../../continuity-equation.md) is

$$
\boxed{\partial_t\rho+\nabla\cdot(\rho\mathbf u)=0,\qquad\frac{D\rho}{Dt}+\rho\nabla\cdot\mathbf u=0.}
$$

For positive [mass density](../../../../../density.md), the [incompressibility condition](../../../../../incompressible-flow.md) $D\rho/Dt=0$ reduces this to $\nabla\cdot\mathbf u=0$. [Mass conservation](../../../../../mass-conservation.md) itself does not require [incompressible flow](../../../../../incompressible-flow.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
