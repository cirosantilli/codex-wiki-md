<h1 id="12c/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $s=x^2+y^2>0$. The first two components of the [curl](../../../../../../curl.md) vanish since the horizontal components are independent of $z$ and the last component depends only on $z$. For the third,

$$
\partial_x\left(\frac{x}{s}\right)=\frac{y^2-x^2}{s^2},\qquad\partial_y\left(\frac{-y}{s}\right)=\frac{y^2-x^2}{s^2},
$$

so **this is a [curl-free vector field](../../../../../../irrotational-vector-field.md) everywhere in its domain**:

$$
\boxed{\nabla\times\mathbf F=0.}
$$

Choose the orientation in which the projection onto the $xy$-plane runs counterclockwise, and parametrize

$$
\mathbf x(t)=(\cos t,\sin t,200+\cos t),\qquad0\leq t\leq2\pi.
$$

On this curve the horizontal contribution is $(-\sin t,\cos t)\cdot(-\sin t,\cos t)\,dt=dt$, while the vertical contribution is $z\,dz=d(z^2/2)$. Its integral over a closed curve is zero. **Therefore**

$$
\boxed{\oint_C\mathbf F\cdot d\mathbf x=2\pi,}
$$

with $-2\pi$ for the opposite orientation. This does not contradict [Stokes theorem](../../../../../../stokes-theorem.md): the planar disk spanning this curve meets the excluded $z$-axis at $(0,0,200)$, where the [vector field](../../../../../../vector-field.md) is undefined. The horizontal one-form is the angular differential and records one winding about that axis; thus this [curl-free vector field](../../../../../../irrotational-vector-field.md) has no single-valued global [potential of a conservative vector field](../../../../../../potential-of-a-conservative-vector-field.md) on its domain.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [12C](../../12c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
