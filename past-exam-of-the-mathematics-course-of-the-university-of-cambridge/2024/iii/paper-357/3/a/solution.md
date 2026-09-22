<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [retarded and advanced null coordinates](../../../../../../retarded-and-advanced-null-coordinates.md) invert to

$$
t=\frac{u+v}{2},\qquad z=\frac{v-u}{2}.
$$

Thus

$$
-dt^2+dz^2=-du\,dv
$$

and the [Minkowski metric](../../../../../../minkowski-metric.md) becomes

$$
\boxed{ds^2=-du\,dv+dx^2+dy^2.}
$$

The [coordinate basis](../../../../../../coordinate-basis.md) transforms by the chain rule:

$$
\boxed{
\partial_t=\partial_u+\partial_v,\qquad
\partial_z=-\partial_u+\partial_v,
}
$$

or equivalently

$$
\boxed{
\partial_u=\frac12(\partial_t-\partial_z),\qquad
\partial_v=\frac12(\partial_t+\partial_z).
}
$$

In the $(z,t)$ diagram, $\partial_t$ points vertically upward and $\partial_z$ horizontally right. The vector $\partial_u$ points along the future-left null ray and $\partial_v$ along the future-right null ray; their factors of one half affect length in the coordinate drawing but not direction.

Using these derivative relations, the [Minkowski wave operator in null coordinates](../../../../../../minkowski-wave-operator-in-null-coordinates.md) is

$$
\boxed{
\Box=-\partial_t^2+\partial_z^2+\partial_x^2+\partial_y^2
=-4\partial_u\partial_v+\partial_x^2+\partial_y^2.
}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 357](../../../paper-357-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
