<h1 id="section-b/7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md) the [spherical cap](../../../../../../spherical-cap.md) has $1<z<\sqrt2$, $0<r<\sqrt{2-z^2}$ and $0<\theta<2\pi$. Its [mass density](../../../../../../density.md) is $kz$ and the [volume element](../../../../../../volume-element.md) is $r\,dr\,d\theta\,dz$. Therefore

$$
M=\int_1^{\sqrt2}\int_0^{2\pi}\int_0^{\sqrt{2-z^2}}kzr\,dr\,d\theta\,dz=\pi k\int_1^{\sqrt2}z(2-z^2)\,dz=\boxed{\frac{\pi k}{4}}.
$$

This is the [mass of a spherical cap with height-proportional density](../../../../../../mass-of-a-spherical-cap-with-height-proportional-density.md) with $R=\sqrt2$ and $c=1$.

For its curved [surface area](../../../../../../surface-area.md), write $z=\sqrt{2-r^2}$ with $0\leq r\leq1$. The [surface integral](../../../../../../surface-integral.md) of one becomes

$$
A=\int_0^{2\pi}\int_0^1\sqrt{1+\left(\frac{dz}{dr}\right)^2}\,r\,dr\,d\theta=2\pi\sqrt2\int_0^1\frac{r}{\sqrt{2-r^2}}\,dr=\boxed{2\pi(2-\sqrt2)}.
$$

It agrees with the [curved area of a spherical cap](../../../../../../curved-area-of-a-spherical-cap.md), $2\pi Rh$, for $h=\sqrt2-1$. The planar closing disk is not part of the requested curved surface.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
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
