<h1 id="3c/solution">Solution</h1>

↑ **Parent:** [3C](../3c.md)

Write $r^2=x^2+y^2$. The first two components have no $z$ dependence, and the third component is zero. The only possibly nonzero component of the [curl](../../../../../curl.md) is

$$
\partial_xF_y-\partial_yF_x=\frac{y^2-x^2}{(x^2+y^2)^2}-\frac{y^2-x^2}{(x^2+y^2)^2}=0.
$$

Thus **$\nabla\times\mathbf F=0$ wherever the field is defined**.

The disk spanning $\gamma_1$ lies away from the excluded axis: the distance from its center to that axis is $2\sqrt2>1$. The field is continuously differentiable on a neighborhood of that disk. The [Stokes theorem](../../../../../stokes-theorem.md) therefore gives

$$
\boxed{\oint_{\gamma_1}\mathbf F\cdot d\mathbf x=0.}
$$

This value is independent of the choice of orientation.

For $\gamma_2$, take the counterclockwise orientation viewed from positive $z$. Put $\mathbf x(t)=(\cos t,\sin t,0)$, $0\leq t\leq2\pi$. Then $\mathbf F(\mathbf x(t))=(-\sin t,\cos t,0)=\mathbf x'(t)$, so the [line integral](../../../../../line-integral.md) is

$$
\boxed{\oint_{\gamma_2}\mathbf F\cdot d\mathbf x=\int_0^{2\pi}1\,dt=2\pi.}
$$

Clockwise orientation gives $-2\pi$; no orientation is printed for this curve. There is no contradiction with the [Stokes theorem](../../../../../stokes-theorem.md): its usual spanning disk intersects the axis where the field is undefined, so the differentiability hypothesis fails. This is a [curl-free vector field](../../../../../irrotational-vector-field.md) with nonzero circulation around the excluded axis; local angular potentials cannot be combined into a single-valued global potential.

## ↑ Ancestors (10)

1. [3C](../3c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
