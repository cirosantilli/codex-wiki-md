<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\Delta G=+\delta^{(3)}$, the [fundamental solution of the Laplace equation](../../../../../fundamental-solution-of-the-laplace-equation.md) in three dimensions is

$$
\boxed{G_0(\mathbf r,\mathbf r')=-\frac1{4\pi|\mathbf r-\mathbf r'|}}.
$$

Its sign follows from the flux: on a small sphere of radius $\varepsilon$, its outward radial [derivative](../../../../../derivative.md) is $1/(4\pi\varepsilon^2)$, with total flux one.

Let $s=|\mathbf r'|\in(0,1)$ and put the image point at $\mathbf r'^*=\mathbf r'/s^2$. The [method of images](../../../../../method-of-images.md) gives the [Dirichlet Green function inside a sphere](../../../../../dirichlet-green-function-inside-a-sphere.md):

$$
\boxed{G_B(\mathbf r,\mathbf r')=-\frac1{4\pi}
\left[\frac1{|\mathbf r-\mathbf r'|}-\frac1{s|\mathbf r-\mathbf r'^*|}\right]}.
$$

The image lies outside the ball, so its potential is harmonic inside. On $|\mathbf r|=1$, the identity $|\mathbf r-\mathbf r'|=s|\mathbf r-\mathbf r'^*|$ makes the two terms cancel. The original source retains unit strength. For a source at the centre, take the limit:

$$
\boxed{G_B(\mathbf r,0)=-\frac1{4\pi}\left(\frac1{|\mathbf r|}-1\right)}.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
