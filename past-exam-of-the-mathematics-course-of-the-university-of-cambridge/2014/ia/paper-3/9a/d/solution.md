<h1 id="9a/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Close the truncated two-sheet [double circular cone](../../../../../../double-circular-cone.md) by the lateral [circular cylinder](../../../../../../circular-cylinder.md) $r=1$, $-1\le z\le1$. Together these form the boundary of the solid in part (c); no planar caps are required because the cone meets the [circular cylinder](../../../../../../circular-cylinder.md) along both end circles. On the [circular cylinder](../../../../../../circular-cylinder.md) the outward unit normal is $(\cos\theta,\sin\theta,0)$, so $\mathbf F\cdot\mathbf n=1$, and $dS=d\theta\,dz$. Its [flux integral](../../../../../../flux-integral.md) is

$$
\int_{-1}^1\int_0^{2\pi}1\,d\theta\,dz=4\pi.
$$

The [divergence theorem](../../../../../../divergence-theorem.md) now gives $\int_S\mathbf F\cdot d\mathbf S+4\pi=4\pi$, using the volume integral from part (c). Hence

$$
\boxed{\int_S\mathbf F\cdot d\mathbf S=0,}
$$

agreeing with tangency. The isolated vertex can be handled by excising a ball of radius $\varepsilon$ and passing to the limit: since $|\mathbf F|=O(\varepsilon)$ there and the added area is $O(\varepsilon^2)$, its extra flux is $O(\varepsilon^3)$ and tends to zero.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [9A](../../9a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
