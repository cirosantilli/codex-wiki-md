<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [curl of a cross product](../../../../../curl-of-a-cross-product.md), the Cartesian contraction is

$$
[\nabla\times(\mathbf w\times\mathbf u)]_i=\epsilon_{ijk}\epsilon_{k\ell m}\partial_j(w_\ell u_m)=\partial_j(w_i u_j-w_j u_i).
$$

The [product rule](../../../../../product-rule.md) then gives

$$
\boxed{\nabla\times(\mathbf w\times\mathbf u)=(\mathbf u\cdot\nabla)\mathbf w+(\nabla\cdot\mathbf u)\mathbf w-(\nabla\cdot\mathbf w)\mathbf u-(\mathbf w\cdot\nabla)\mathbf u.}
$$

For the fluid equation, replace the advective term by $\mathbf w\times\mathbf u+\nabla(|\mathbf u|^2/2)$ using the preceding identity. Take its curl. Both gradient terms have zero curl, while $\nabla\cdot\mathbf w=\nabla\cdot(\nabla\times\mathbf u)=0$ and incompressibility gives $\nabla\cdot\mathbf u=0$. The [vorticity equation](../../../../../vorticity-equation.md) is consequently

$$
\boxed{\partial_t\mathbf w+(\mathbf u\cdot\nabla)\mathbf w=(\mathbf w\cdot\nabla)\mathbf u.}
$$

The left side is the [material derivative](../../../../../material-derivative.md) of [vorticity](../../../../../vorticity-split.md); the right is [vortex stretching](../../../../../vortex-stretching.md). It follows here because the given force per mass is a gradient, in addition to the flow being inviscid and incompressible.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
