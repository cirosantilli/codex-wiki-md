<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For $h=x^2/a^2+y^2/b^2+z^2-1$, the [gradient](../../../../gradient.md) $\nabla h=2(x/a^2,y/b^2,z)$ is a [normal vector](../../../../normal-vector.md) to the [ellipsoid](../../../../ellipsoid.md). The outward [unit normal vector](../../../../unit-normal.md) is $(x/a^2,y/b^2,z)/\sqrt{x^2/a^4+y^2/b^4+z^2}$. The conditions $a,b>\sqrt2$ ensure that $z=\sqrt{1-x^2/a^2-y^2/b^2}>0$ everywhere on the rectangular projection.

The [dot product](../../../../dot-product.md) $F\cdot\nabla h=2xy(1/b^2-1/a^2)$ vanishes pointwise when $a=b$. In that case $F$ has no normal component, so **the [surface flux](../../../../flux-integral.md) is zero**. For unequal axes, the given [vector surface element](../../../../vector-area-element.md) gives

$$
\Phi=\left(\frac1{b^2}-\frac1{a^2}\right)\int_0^1\int_0^1\frac{xy}{\sqrt{1-x^2/a^2-y^2/b^2}}\,dy\,dx.
$$

Put $u=x^2/a^2$, $v=y^2/b^2$. Then $xy\,dxdy=a^2b^2\,dudv/4$, and

$$
\Phi=\frac{a^2-b^2}{4}\int_0^{1/a^2}\int_0^{1/b^2}(1-u-v)^{-1/2}\,dv\,du.
$$

Two elementary [integrations](../../../../integral-split.md) now give

$$
\boxed{\Phi=\frac{a^2-b^2}{3}\left[1-\left(1-\frac1{a^2}\right)^{3/2}-\left(1-\frac1{b^2}\right)^{3/2}+\left(1-\frac1{a^2}-\frac1{b^2}\right)^{3/2}\right].}
$$

This is the [rotational flux through an ellipsoidal graph patch](../../../../rotational-flux-through-an-ellipsoidal-graph-patch.md) with unit vertical semiaxis and unit projection lengths. It also tends continuously to zero when $a=b$, agreeing with the pointwise argument.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Paper 2](../../paper-2-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
