<h1 id="section-b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For positive semiaxes $a,b$, the [cross product](../../../../../../cross-product.md) of the two parametric [tangent vectors](../../../../../../tangent-vector-split.md) gives the outward [oriented surface element of an ellipsoid of revolution](../../../../../../oriented-surface-element-of-an-ellipsoid-of-revolution.md):

$$
\mathbf x_\theta\times\mathbf x_\phi=(ab\sin^2\theta\cos\phi,\ ab\sin^2\theta\sin\phi,\ b^2\sin\theta\cos\theta).
$$

Substituting the parametrization into the [vector field](../../../../../../vector-field.md) and taking its [dot product](../../../../../../dot-product.md) with this element gives

$$
\mathbf G\cdot(\mathbf x_\theta\times\mathbf x_\phi)=a^3b^2\sin^3\theta\cos^2\theta\cos^2\phi+ab^4\sin^5\theta\cos\phi\sin^3\phi+a^3b^2\sin\theta\cos^4\theta.
$$

The middle term has zero [integral](../../../../../../integral-split.md) over $0\leq\phi\leq2\pi$. In the other terms, $\int_0^{2\pi}\cos^2\phi\,d\phi=\pi$, $\int_0^\pi\sin^3\theta\cos^2\theta\,d\theta=4/15$, and $\int_0^\pi\sin\theta\cos^4\theta\,d\theta=2/5$. The directly evaluated [flux](../../../../../../flux.md) is therefore

$$
\boxed{\int_S\mathbf G\cdot d\mathbf S=a^3b^2\left(\frac{4\pi}{15}+\frac{4\pi}{5}\right)=\frac{16\pi a^3b^2}{15}.}
$$

## ↑ Ancestors (14)

1. [D](../d.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
