<h1 id="13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the [scalar field](../../../../../scalar-field.md) as $u=R(r)Y(\theta,\phi)$, where $R=r+r^{-2}$ and $Y=\sin\theta\cos\phi$. Its radial contribution to the [Laplacian](../../../../../laplacian.md) in [spherical coordinates](../../../../../spherical-coordinate-system.md) is

$$
\frac{Y}{r^2}(r^2R')'=Y\left(\frac2r+\frac2{r^4}\right)=\frac{2R}{r^2}Y.
$$

For the angular contribution, $Y_\theta=\cos\theta\cos\phi$ and $Y_{\phi\phi}=-\sin\theta\cos\phi$, so

$$
\frac1{\sin\theta}\partial_\theta(\sin\theta\,Y_\theta)
+\frac{Y_{\phi\phi}}{\sin^2\theta}
=\frac{\cos\phi}{\sin\theta}(\cos^2\theta-\sin^2\theta-1)=-2Y.
$$

Combining the radial and angular terms proves

$$
\boxed{\nabla^2u=\frac{2R}{r^2}Y-\frac{2R}{r^2}Y=0\qquad(r>0).}
$$

The calculation uses $0<\theta<\pi$ to avoid coordinate singularities. In [Cartesian coordinates](../../../../../cartesian-coordinate-system.md), $u=x(1+r^{-3})$, which extends smoothly across the polar axis for $r>0$. It therefore satisfies [Laplace's equation](../../../../../laplace-equation.md) there as well. The origin is a genuine singularity and is excluded.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
