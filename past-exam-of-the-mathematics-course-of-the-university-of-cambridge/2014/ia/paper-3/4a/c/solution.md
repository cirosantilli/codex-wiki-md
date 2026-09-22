<h1 id="4a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $\gamma(t)=(\cos t,\sin t,0)$ for $0\le t\le2\pi$. On this path $\mathbf F=(-\sin t,\cos t,0)=\gamma'(t)$, so its [line integral](../../../../../../line-integral.md) is

$$
\boxed{\oint_\gamma\mathbf F\cdot d\mathbf x=\int_0^{2\pi}1\,dt=2\pi.}
$$

The first two components of the [curl](../../../../../../curl.md) vanish because the field is independent of $z$ and has zero third component. Writing $q=x^2+y^2$, its third [curl](../../../../../../curl.md) component is

$$
\partial_x(x/q)-\partial_y(-y/q)
=\frac{y^2-x^2}{q^2}-\frac{y^2-x^2}{q^2}=0.
$$

Thus this [azimuthal inverse-radius vector field](../../../../../../azimuthal-inverse-radius-vector-field.md) is a [curl-free vector field](../../../../../../irrotational-vector-field.md) on $G=\mathbb R^3\setminus\{(0,0,z):z\in\mathbb R\}$, but its [line integral](../../../../../../line-integral.md) is not path independent. This domain is not [simply connected](../../../../../../simply-connected-space.md): the circle links the removed axis. A spanning disk through the axis is inadmissible for [Stokes theorem](../../../../../../stokes-theorem.md), since the [vector field](../../../../../../vector-field.md) is undefined there. **Zero [curl](../../../../../../curl.md) alone does not force global path independence.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4A](../../4a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
