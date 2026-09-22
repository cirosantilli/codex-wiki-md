<h1 id="25i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $h(r,\theta)=\sqrt{G(r,\theta)}$. The [Jacobi equation in geodesic polar coordinates](../../../../../../jacobi-equation-in-geodesic-polar-coordinates.md) and the initial conditions from part (b) are

$$
h_{rr}=-Kh,
\qquad h(0,\theta)=0,
\qquad h_r(0,\theta)=1.
$$

Inside a geodesic polar coordinate ball, $h>0$. If $K\leq0$, then $h_{rr}\geq0$, so $h_r\geq1$ and therefore $h(r,\theta)\geq r$. The [Riemannian area element](../../../../../../area-element-of-a-surface.md) is $h\,dr\,d\theta$, whence

$$
\operatorname{Area}B(p,\varepsilon_0)
=\int_0^{2\pi}\int_0^{\varepsilon_0}h(r,\theta)\,dr\,d\theta
\geq\int_0^{2\pi}\int_0^{\varepsilon_0}r\,dr\,d\theta
=\pi\varepsilon_0^2.
$$

**Thus nonpositive [Gaussian curvature](../../../../../../gaussian-curvature.md) makes such a ball at least as large as the [Euclidean disk](../../../../../../disk-mathematics.md) of the same radius.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [25I](../../25i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
