<h1 id="3/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Reflect $r'=(x',y',z')$ to $r'^*=(x',y',-z')$. The [method of images](../../../../../../method-of-images.md) gives the [Dirichlet image kernel for the three-dimensional Helmholtz equation](../../../../../../dirichlet-image-kernel-for-the-three-dimensional-helmholtz-equation.md):

$$
\boxed{G_D(r,r')=-\frac1{4\pi}\left[\frac{e^{ik|r-r'|}}{|r-r'|}-\frac{e^{ik|r-r'^*|}}{|r-r'^*|}\right].}
$$

The two distances coincide on the plane, so its boundary value is zero; the image source is outside the domain. It therefore has the required positive delta source inside and the selected outgoing behaviour.

Let $h(R)=e^{ikR}/R$. At a boundary point $r=(\xi,\eta,0)$, the distances to the real and reflected sources have $z$ derivatives $-z'/R$ and $+z'/R$. Thus

$$
\partial_zG_D=\frac{z'}{2\pi R}h'(R),\qquad h'(R)=\frac{e^{ikR}}R\left(ik-\frac1R\right).
$$

The outward [unit normal](../../../../../../unit-normal.md) of the upper half-space is $-e_z$, and $z'/R=\cos\theta$. Hence

$$
\partial_nG_D=-\frac{ik}{2\pi}\frac{e^{ikR}}R\left(1+\frac{i}{kR}\right)\cos\theta.
$$

Using the decay assumption to discard the distant hemisphere in the boundary representation gives

$$
\boxed{\phi(r')=-\frac{ik}{2\pi}\int_{z=0}\frac{e^{ikR}}R\left(1+\frac{i}{kR}\right)\cos\theta\,\phi(r)\,dS.}
$$

The qualification at infinity concerns the whole Green boundary term, not just the pointwise limit of $\phi$. Sufficient decay of the field and its derivatives, as assumed, makes it vanish; compatible radiation conditions can also do so. As a sign check, taking $k\to0$ in the kernel gives $z'/(2\pi R^3)$, the positive [Poisson kernel for the upper half-space](../../../../../../poisson-kernel-for-the-upper-half-space.md).

## ↑ Ancestors (14)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [3](../../../3.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
