<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On the radius-$a$ sphere, the outward unit [normal vector](../../../../../normal-vector.md) is $(x,y,z)/a$, so $\mathbf F\cdot\mathbf n=(x^2+2y^2+3z^2)/a$. For a direct [surface integral](../../../../../surface-integral.md), put $x=a\sin\theta\cos\varphi$, $y=a\sin\theta\sin\varphi$, $z=a\cos\theta$ and $dS=a^2\sin\theta\,d\theta\,d\varphi$. The integral is

$$
a^3\int_0^{2\pi}\!\int_0^\pi[\sin^2\theta(\cos^2\varphi+2\sin^2\varphi)+3\cos^2\theta]\sin\theta\,d\theta\,d\varphi.
$$

The azimuthal integrals are $\pi,\pi,2\pi$, while $\int_0^\pi\sin^3\theta\,d\theta=4/3$ and $\int_0^\pi\cos^2\theta\sin\theta\,d\theta=2/3$. Thus

$$
\boxed{\int_S\mathbf F\cdot d\mathbf S=a^3\left[3\pi\frac43+6\pi\frac23\right]=8\pi a^3.}
$$

The [flux of a linear field through a sphere](../../../../../flux-of-a-linear-field-through-a-sphere.md) also follows from the equality of the three spherical second moments, without using the [divergence theorem](../../../../../divergence-theorem.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
