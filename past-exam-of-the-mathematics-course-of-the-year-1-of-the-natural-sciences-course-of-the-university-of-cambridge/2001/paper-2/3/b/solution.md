<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On the [circular cylinder](../../../../../circular-cylinder.md), $\rho=R$ is constant, so the given [line element](../../../../../line-element.md) reduces to $ds^2=R^2d\phi^2+dz^2$. Unroll the [circular cylinder](../../../../../circular-cylinder.md) with $u=R\phi$. The [line element](../../../../../line-element.md) is then $ds^2=du^2+dz^2$, so the usual [Euclidean geometry](../../../../../euclidean-geometry-split.md) formula measures [arc length](../../../../../arc-length.md) in the $(u,z)$ [plane](../../../../../plane.md).

The endpoint has infinitely many lifts $(R(\phi_1+2\pi k),z_1)$, with $k\in\mathbb Z$. For each lift, the [straight line](../../../../../straight-line.md) segment is shortest; its [length](../../../../../length.md) is $\sqrt{R^2(\phi_1+2\pi k)^2+z_1^2}$. Comparing the lifts gives the unrestricted [shortest path on a circular cylinder](../../../../../shortest-path-on-a-circular-cylinder.md):

$$
\boxed{L_{\min}=\min_{k\in\mathbb Z}\sqrt{R^2(\phi_1+2\pi k)^2+z_1^2}.}
$$

If $\delta$ is a minimizing angular increment, a shortest [geodesic](../../../../../geodesic.md) is parametrized by $(\rho,\phi,z)=(R,\delta t,z_1t)$, $0\leq t\leq1$. This is a [helix](../../../../../helix.md) when both increments are nonzero, and a circular arc or vertical generator in the limiting cases. A nonminimal lift also gives a [geodesic](../../../../../geodesic.md), but it is only shortest within its fixed winding class.

For $0\leq\phi_1\leq2\pi$, put $m=\min(\phi_1,2\pi-\phi_1)$. Then $\boxed{L_{\min}=\sqrt{R^2m^2+z_1^2}}$. At $\phi_1=\pi$, both winding directions give distinct shortest paths of equal [length](../../../../../length.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
