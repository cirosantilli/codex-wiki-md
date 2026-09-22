# Maximum-volume cuboid in a hemisphere

↑ **Parent:** [Hemisphere](hemisphere.md)

For a closed [hemisphere](hemisphere.md) of [radius](radius.md) $a>0$, take a [rectangular parallelepiped](rectangular-parallelepiped.md) with a face on the flat base, base half-widths $x,y>0$ and height $z>0$. Its curved-boundary constraint is $x^2+y^2+z^2=a^2$ and its [volume](volume.md) is $4xyz$. A [Lagrange multiplier](lagrange-multiplier.md) gives $x=y=z=a/\sqrt3$, yielding the displayed maximum. The full edge lengths are $2a/\sqrt3,2a/\sqrt3,a/\sqrt3$.

This bound remains valid when arbitrary orientations are allowed. Write a cuboid's half-edge lengths as $u_1,u_2,u_3$, its center components in its orthonormal edge basis as $v_i$, and the vertical unit-vector components as $n_i$. Containment above the base plane requires $\sum n_iv_i\geq\sum|n_i|u_i$. Hence $|v_j|\geq u_j$ for at least one $j$: otherwise every contributing term would be strictly smaller than its required bound. Its farthest vertex has squared distance

$$
\sum_i u_i^2+\sum_i v_i^2+2\sum_i u_i|v_i|
\geq\sum_{i\ne j}u_i^2+4u_j^2.
$$

Containment in the sphere bounds the right side by $a^2$. The [arithmetic-geometric mean inequality](arithmetic-geometric-mean-inequality.md) then gives $2u_1u_2u_3\leq a^3/(3\sqrt3)$, so the full [volume](volume.md) $8u_1u_2u_3$ cannot exceed the displayed value. The constructed cuboid attains it. With strict containment and no boundary contact, the same value is a supremum.

## ↑ Ancestors (7)

1. [Hemisphere](hemisphere.md)
2. [Sphere](sphere.md)
3. [Euclidean geometry](euclidean-geometry-split.md)
4. [Geometry and topology](geometry-and-topology-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/20/a/solution.md)
