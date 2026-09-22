<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Reflect the physical source across $z=0$, writing $\overline{\mathbf r'}=(x',y',-z')$. Its radius is still $s=|\mathbf r'|$, and its spherical image is $\overline{\mathbf r^*}$. The [Dirichlet Green function inside a hemisphere](../../../../../dirichlet-green-function-inside-a-hemisphere.md) is

$$
\boxed{G_1(\mathbf r,\mathbf r')=G_0(\mathbf r,\mathbf r')-G_0(\mathbf r,\overline{\mathbf r'}).}
$$

Explicitly this four-source [method of images](../../../../../method-of-images.md) is

$$
G_1=-\frac1{4\pi}\left[
\frac1{|\mathbf r-\mathbf r'|}-\frac1{|\mathbf r-\overline{\mathbf r'}|}
-\frac1{s|\mathbf r-\mathbf r^*|}+\frac1{s|\mathbf r-\overline{\mathbf r^*}|}\right].
$$

Both $G_0$ terms vanish on the spherical cap. On the flat equatorial disc, reflection equates the two physical-source distances and also the two image-source distances, so both pairs cancel. The reflected physical source lies in the lower half-ball and the two inverted images lie outside the sphere. Consequently the only source in the upper half-ball is $\mathbf r'$, with the correct coefficient:

$$
\boxed{\Delta_{\mathbf r}G_1=\delta(\mathbf r-\mathbf r'),\qquad G_1=0\text{ on both boundary pieces}.}
$$

The [Dirichlet uniqueness for the Poisson equation](../../../../../dirichlet-uniqueness-for-the-poisson-equation.md) then identifies this as the required Green function.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
