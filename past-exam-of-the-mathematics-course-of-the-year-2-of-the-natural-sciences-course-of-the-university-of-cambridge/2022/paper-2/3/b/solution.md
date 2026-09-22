<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The three-dimensional [fundamental solution of the Laplace equation](../../../../../fundamental-solution-of-the-laplace-equation.md), with $\Delta F=+\delta$, is

$$
\boxed{F(\mathbf r,\mathbf r')=-\frac1{4\pi|\mathbf r-\mathbf r'|}.}
$$

It is [harmonic](../../../../../harmonic-function.md) away from the source, and its gradient has total outward [flux](../../../../../flux.md) one through a small source-centred sphere.

For $s=|\mathbf r'|\in(0,1)$, place the image at $\mathbf r^*=\mathbf r'/s^2$, outside the unit ball. On $|\mathbf r|=1$, expansion of squared distances gives $|\mathbf r-\mathbf r^*|=|\mathbf r-\mathbf r'|/s$. The [method of images](../../../../../method-of-images.md) therefore gives the [Dirichlet Green function inside a sphere](../../../../../dirichlet-green-function-inside-a-sphere.md)

$$
\boxed{G_0(\mathbf r,\mathbf r')=-\frac1{4\pi}\left[\frac1{|\mathbf r-\mathbf r'|}-\frac1{s|\mathbf r-\mathbf r^*|}\right].}
$$

The boundary value is zero by the distance identity, and the image term is harmonic throughout the physical ball. Thus $\Delta G_0=\delta(\mathbf r-\mathbf r')$ there. At the central source, take the finite limit of the weighted image term:

$$
\boxed{G_0(\mathbf r,0)=-\frac1{4\pi|\mathbf r|}+\frac1{4\pi}.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
