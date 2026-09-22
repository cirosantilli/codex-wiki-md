<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [Dirichlet Green function](../../../../../dirichlet-green-function.md) satisfies $\Delta_{\mathbf x}G_D(\mathbf x,\mathbf y)=\delta^{(2)}(\mathbf x-\mathbf y)$ in the domain and $G_D=0$ when $\mathbf x$ lies on its boundary. For a source $\mathbf y\ne0$ in the [unit disc](../../../../../unit-disc.md), put its opposite image at $\mathbf y^*=\mathbf y/|\mathbf y|^2$. The [method of images](../../../../../method-of-images.md) gives

$$
\boxed{G_D(\mathbf x,\mathbf y)
=\frac1{2\pi}\log\frac{|\mathbf x-\mathbf y|}{|\mathbf y|\,|\mathbf x-\mathbf y^*|}}.
$$

The image lies outside the [unit disc](../../../../../unit-disc.md), so its logarithm is a [harmonic function](../../../../../harmonic-function.md) inside. The original logarithm has precisely the unit source strength found in part (a). On $|\mathbf x|=1$,

$$
|\mathbf x-\mathbf y|^2
=1-2\mathbf x\cdot\mathbf y+|\mathbf y|^2
=|\mathbf y|^2|\mathbf x-\mathbf y^*|^2,
$$

so the boundary value is zero. Equivalently, in [complex coordinates](../../../../../complex-coordinate.md), the [Dirichlet Green function inside the unit disk](../../../../../dirichlet-green-function-inside-the-unit-disk.md) is

$$
G_D(z,\zeta)=\frac1{2\pi}\log\left|\frac{z-\zeta}{1-z\bar\zeta}\right|.
$$

This also covers a source at the origin, where $G_D(z,0)=(2\pi)^{-1}\log|z|$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
