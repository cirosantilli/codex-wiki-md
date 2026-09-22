<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Reflect the source across the plane, defining $\mathbf r'^*=(x',y',-z')$ for an interior point $z'>0$. Superpose the direct [Green function](../../../../../green-s-function-split.md) from part (b) and an image of opposite sign:

$$
\boxed{\Psi(\mathbf r,\mathbf r')=-\frac1{4\pi}\left[\frac{e^{-\kappa|\mathbf r-\mathbf r'|}}{|\mathbf r-\mathbf r'|}-\frac{e^{-\kappa|\mathbf r-\mathbf r'^*|}}{|\mathbf r-\mathbf r'^*|}\right],\qquad\kappa=|k|.}
$$

The direct term supplies the delta source in the upper half-space; the image singularity lies outside that domain and contributes no source there. On $z=0$ the two distances are equal, so the terms cancel, giving homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md). Both decay at infinity, which is the additional condition selecting this half-space solution. This is the [method of images](../../../../../method-of-images.md) realization of the [Dirichlet image kernel for the three-dimensional modified Helmholtz equation](../../../../../dirichlet-image-kernel-for-the-three-dimensional-modified-helmholtz-equation.md). It includes the unscreened case $k=0$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
