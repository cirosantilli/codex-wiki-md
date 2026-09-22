<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $f=u+iv$ and $z=x+iy$. For a positively oriented, piecewise smooth simple closed [contour](../../../../../complex-integration-contour.md) bounding a region where $u,v$ have continuous first [partial derivatives](../../../../../partial-derivative.md), [Green's theorem](../../../../../green-theorem.md) gives

$$
\begin{aligned}
\oint_C f(z)\,dz
&=\oint_C(u\,dx-v\,dy)+i\oint_C(v\,dx+u\,dy)\\
&=\iint_S(-v_x-u_y)\,dx\,dy+i\iint_S(u_x-v_y)\,dx\,dy.
\end{aligned}
$$

The [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) are $u_x=v_y$ and $u_y=-v_x$, so both integrands vanish:

$$
\boxed{\oint_C f(z)\,dz=0.}
$$

This proves [Cauchy's integral theorem](../../../../../cauchy-s-integral-theorem.md) under the standard regularity assumptions for [Green's theorem](../../../../../green-theorem.md). More general admissible [contours](../../../../../complex-integration-contour.md) follow by subdivision; every enclosed region must be free of singularities.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
