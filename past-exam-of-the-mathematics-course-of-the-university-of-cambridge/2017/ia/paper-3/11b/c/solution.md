<h1 id="11b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [directional derivative](../../../../../../directional-derivative.md) along the specified [vector field](../../../../../../vector-field.md) gives

$$
(\mathbf F\cdot\nabla)\mathbf F=(x,y,z),\qquad
\mathbf F\times(\mathbf F\cdot\nabla)\mathbf F=(2yz,-2xz,0).
$$

Use the magnitude formula for the [curvature of an integral curve of a vector field](../../../../../../curvature-of-an-integral-curve-of-a-vector-field.md):

$$
\boxed{\kappa(x,y,z)=\frac{2|z|\sqrt{x^2+y^2}}{(x^2+y^2+z^2)^{3/2}},\qquad (x,y,z)\ne(0,0,0).}
$$

It vanishes on the [plane](../../../../../../plane.md) $z=0$ and on the $z$ axis away from the origin, consistent with straight field lines there. At the origin the [vector field](../../../../../../vector-field.md) vanishes, so it fails the nowhere-zero hypothesis and this field-line curvature is not defined.

As an independent geometric check, an [integral curve of a vector field](../../../../../../integral-curve-of-a-vector-field.md) satisfies $\dot x=x$, $\dot y=y$, $\dot z=-z$, giving $(x,y,z)=(ae^u,be^u,ce^{-u})$. Its velocity is $(x,y,-z)$ and acceleration $(x,y,z)$; the ordinary [curvature of a space curve](../../../../../../curvature-of-a-space-curve.md) formula $|r'\times r''|/|r'|^3$ gives the same expression.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11B](../../11b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
