<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a regular [parametric surface](../../../../parametric-surface.md) $\mathbf r(u,v)$, its [tangent vectors](../../../../tangent-vector-split.md) $\mathbf r_u,\mathbf r_v$ are linearly independent. The [first fundamental form](../../../../first-fundamental-form.md) is the induced [inner product](../../../../inner-product-split.md) on the [tangent plane](../../../../tangent-plane.md), written

$$
I=E\,du^2+2F\,du\,dv+G\,dv^2,\qquad
E=\mathbf r_u\cdot\mathbf r_u,\quad F=\mathbf r_u\cdot\mathbf r_v,\quad G=\mathbf r_v\cdot\mathbf r_v.
$$

It measures squared [lengths](../../../../length.md) and [angles](../../../../angle.md); its [determinant](../../../../determinant.md) satisfies $EG-F^2=|\mathbf r_u\times\mathbf r_v|^2>0$. Choose the [unit normal](../../../../unit-normal.md)

$$
N=\frac{\mathbf r_u\times\mathbf r_v}{\sqrt{EG-F^2}}.
$$

The [second fundamental form](../../../../second-fundamental-form-split.md), with [shape operator](../../../../shape-operator.md) $S=-dN$, is

$$
II=e\,du^2+2f\,du\,dv+g_2\,dv^2,\qquad
e=\mathbf r_{uu}\cdot N,\quad f=\mathbf r_{uv}\cdot N,\quad g_2=\mathbf r_{vv}\cdot N.
$$

The subscript distinguishes the coefficient $g_2$ from a [genus](../../../../genus-of-a-surface.md) or a [Riemannian metric](../../../../riemannian-metric-split.md). In these coordinates the [shape operator](../../../../shape-operator.md) has matrix $I^{-1}II$, so the [Gaussian curvature](../../../../gaussian-curvature.md), the product of its two [principal curvatures](../../../../principal-curvature.md), is

$$
\boxed{\kappa=\det S=\frac{eg_2-f^2}{EG-F^2}.}
$$

Reversing $N$ reverses $II$ and both [principal curvatures](../../../../principal-curvature.md), leaving the [Gaussian curvature](../../../../gaussian-curvature.md) unchanged.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the geometry of surfaces course of the University of Oxford](../../../split.md)
5. [Geometry of surfaces course of the University of Oxford](../../../../geometry-of-surfaces-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
