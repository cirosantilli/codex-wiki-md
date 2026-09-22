# Vector calculus in elliptic cylindrical coordinates

↑ **Parent:** [Elliptic cylindrical coordinates](elliptic-cylindrical-coordinates.md)

In [elliptic cylindrical coordinates](elliptic-cylindrical-coordinates.md), write a [vector field](vector-field.md) as $A=A_u e_u+A_v e_v+A_z e_z$ using the local orthonormal [unit vectors](unit-vector.md). The [scale factors of orthogonal coordinates](scale-factors-of-orthogonal-coordinates.md) are $(h,h,1)$, so the [divergence](divergence.md) and [curl](curl.md) are

$$
\nabla\cdot A=\frac{\partial_u(hA_u)+\partial_v(hA_v)+\partial_z(h^2A_z)}{h^2},
$$



$$
\nabla\times A=\frac{\partial_vA_z-\partial_z(hA_v)}h e_u+\frac{\partial_z(hA_u)-\partial_uA_z}h e_v+\frac{\partial_u(hA_v)-\partial_v(hA_u)}{h^2}e_z.
$$

Applying the [divergence](divergence.md) to the [gradient](gradient.md) of a scalar [function](function-split.md) gives $\Delta\phi=(\phi_{uu}+\phi_{vv})/h^2+\phi_{zz}$. These formulas hold where $h>0$. They use physical components along [unit vectors](unit-vector.md), rather than components along the unnormalized coordinate [tangent vectors](tangent-vector-split.md).

## ↑ Ancestors (10)

1. [Elliptic cylindrical coordinates](elliptic-cylindrical-coordinates.md)
2. [Orthogonal coordinates](orthogonal-coordinates.md)
3. [Change of variables formula](change-of-variables-formula.md)
4. [Multivariable calculus](multivariable-calculus-split.md)
5. [Calculus](calculus-split.md)
6. [Real analysis](real-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1/1/solution.md)
