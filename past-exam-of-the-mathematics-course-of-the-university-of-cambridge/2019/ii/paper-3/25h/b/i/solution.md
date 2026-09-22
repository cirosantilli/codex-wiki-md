<h1 id="25h/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Because $f'(a)$ and $f'(b)$ are nonzero, $r=f(v)$ is a valid one-sided local coordinate at each endpoint. Define

$$
h_a(r)=g\bigl(f^{-1}(r)\bigr)
$$

using the inverse near $a$, and define $h_b$ analogously near $b$. The necessary and sufficient conditions are:


- $g(a)\ne g(b)$, so the two collapsed boundary circles give two distinct poles;
- near each endpoint there is a smooth function $H_*$ such that


$$
h_*(r)=h_*(0)+H_*(r^2).
$$

Indeed, the second condition makes the surface near the corresponding pole the graph

$$
z=h_*(0)+H_*(x^2+y^2),
$$

which is a smooth regular graph over the horizontal tangent plane. Together with part a(i), these two pole charts cover the closure by [regular surface](../../../../../../../smooth-surface.md) charts. The surface is compact because it is the continuous image of the compact cylinder $[0,2\pi]\times[a,b]$ after each boundary circle is collapsed to its pole.

Conversely, rotational invariance forces the tangent plane at a pole to be horizontal. The surface is therefore locally the graph of a smooth radial function of $(x,y)$. A smooth rotation-invariant function near the origin is a smooth function of $x^2+y^2$, which gives the displayed condition. The poles must be distinct, since otherwise a punctured neighbourhood of their common image would have two components and could not be a surface chart. This is the [smooth endpoint criterion for a surface of revolution](../../../../../../../smooth-endpoint-criterion-for-a-surface-of-revolution.md). In particular it implies the familiar first-order conditions $g'(a)=g'(b)=0$, but those conditions alone do not ensure smoothness of every order.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [25H](../../../25h.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
