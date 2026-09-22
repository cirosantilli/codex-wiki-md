<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $m$ be the number of [facets](../../../../../../facet.md) of the [convex polytope](../../../../../../convex-polytope.md) $P$. Its facet description can be written

$$
P=\bigcap_{j=1}^m\{x:u_j\cdot x\leq h_j\},\qquad\lVert u_j\rVert=1.
$$

Because $r^{-1}B^n\subset P$, each supporting [closed half-space](../../../../../../closed-half-space.md) has $h_j\geq1/r$. For any $\theta\in S^{n-1}$, follow the ray $t\theta$ to its last point in $P$. Its radius $t_\theta$ is at most one because $P\subset B^n$. At least one [facet](../../../../../../facet.md) is active there, giving

$$
t_\theta u_j\cdot\theta=h_j\geq1/r,\qquad u_j\cdot\theta\geq1/r.
$$

Thus the [unit sphere](../../../../../../unit-sphere.md) is covered by the $m$ [spherical caps](../../../../../../spherical-cap.md) centred at $u_j$ with angular radius $\rho=\arccos(1/r)$. Since $r\geq\sqrt2$, this radius lies in $[\pi/4,\pi/2)$ and the [spherical cap area upper bound](../../../../../../spherical-cap-area-upper-bound.md) applies. Subadditivity of [surface area](../../../../../../surface-area.md) gives

$$
1\leq m\sin^n\rho=m(1-r^{-2})^{n/2}.
$$

Using $\log(1-x)\leq-x$ for $0<x<1$,

$$
\boxed{m\geq(1-r^{-2})^{-n/2}\geq\exp\!\left(\frac{n}{2r^2}\right).}
$$

**The [facet lower bound for ball approximations](../../../../../../facet-lower-bound-for-ball-approximations.md) is exponential in the dimension.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
