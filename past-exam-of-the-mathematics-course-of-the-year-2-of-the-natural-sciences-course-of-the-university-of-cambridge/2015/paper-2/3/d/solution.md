<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let the evaluation point be $\mathbf r_0=(x,y,z)$, $z>0$, and reflect it to $\mathbf r_0^*=(x,y,-z)$. The [method of images](../../../../../method-of-images.md) constructs

$$
\boxed{G(\mathbf r,\mathbf r_0)=\frac1{4\pi}\left[\frac1{|\mathbf r-\mathbf r_0|}-\frac1{|\mathbf r-\mathbf r_0^*|}\right].}
$$

The two [Euclidean distances](../../../../../euclidean-distance.md) coincide on the plane, so $G=0$ there. The negative image source lies outside the domain; inside, only the real source contributes to $-\nabla_{\mathbf r}^2G=\delta^{(3)}(\mathbf r-\mathbf r_0)$. The difference also decays at infinity.

On the plane write $\mathbf r=(\xi,\eta,s)$ and set $s=0$. The outward [unit normal](../../../../../unit-normal.md) of the upper half-space is $n=-e_z$. Direct differentiation gives

$$
\left.\partial_sG\right|_{s=0}=\frac{z}{2\pi[(x-\xi)^2+(y-\eta)^2+z^2]^{3/2}},\qquad\partial_nG=-\partial_sG.
$$

Substituting into the boundary representation from part (c) yields the [Poisson kernel for the upper half-space](../../../../../poisson-kernel-for-the-upper-half-space.md):

$$
\boxed{\phi(x,y,z)=\frac{z}{2\pi}\int_{\mathbb R^2}\frac{f(\xi,\eta)}{[(x-\xi)^2+(y-\eta)^2+z^2]^{3/2}}\,d\xi\,d\eta.}
$$

Its sign is positive, as expected from the [maximum principle](../../../../../maximum-principle.md) for nonnegative boundary data. Its normalization can be checked in [polar coordinates](../../../../../polar-coordinates.md):

$$
\int_{\mathbb R^2}P_z\,d\xi\,d\eta=z\int_0^\infty\frac{r\,dr}{(r^2+z^2)^{3/2}}=1.
$$

As $z\downarrow0$ the kernel is an [approximate identity](../../../../../approximate-identity.md), recovering $f$ at its continuity points. Boundary data must have the decay and regularity compatible with the stated condition at infinity.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
