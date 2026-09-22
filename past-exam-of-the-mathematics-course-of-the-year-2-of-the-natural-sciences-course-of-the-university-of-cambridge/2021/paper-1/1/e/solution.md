<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For a nondegenerate surface take $R>0$, and abbreviate $C=\cosh R$, $H=\sinh R$. Close the upper [oblate spheroid](../../../../../oblate-spheroid.md) by its equatorial disk $D$, obtaining a half-ellipsoid $V$. The [divergence](../../../../../divergence.md) is

$$
\nabla\cdot\mathbf A=y^2+2y.
$$

The integral of $2y$ vanishes by reflection symmetry. At height $z$, the cross-section is a disk of radius $q=C\sqrt{1-z^2/H^2}$. Using planar [polar coordinates](../../../../../polar-coordinates.md),

$$
\int_{x^2+y^2\leq q^2}y^2\,dx\,dy=\int_0^{2\pi}\sin^2\vartheta\,d\vartheta\int_0^q r^3dr=\frac{\pi q^4}{4}.
$$

Consequently

$$
\int_Vy^2\,dV=\frac{\pi C^4}{4}\int_0^H\left(1-\frac{z^2}{H^2}\right)^2dz=\frac{2\pi}{15}C^4H.
$$

The outward [unit normal vector](../../../../../unit-normal.md) on $D$ is $-\mathbf e_z$, so its [flux](../../../../../flux.md) is $-2\pi C^2$. Applying the [divergence theorem](../../../../../divergence-theorem.md) to the closed surface and subtracting this disk contribution gives

$$
\boxed{\int_S\mathbf A\cdot\mathbf n\,dS=2\pi\cosh^2R+\frac{2\pi}{15}\cosh^4R\sinh R.}
$$

This is a special case of [polynomial flux through a half-ellipsoid](../../../../../polynomial-flux-through-a-half-ellipsoid.md). Including the closing disk is essential: the constant vertical component has zero [divergence](../../../../../divergence.md) but nonzero flux through the open curved surface.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
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
