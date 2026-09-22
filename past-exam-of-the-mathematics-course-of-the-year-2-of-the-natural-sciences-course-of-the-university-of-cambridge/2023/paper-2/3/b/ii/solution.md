<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $s=|\mathbf r'|$ and $\mathbf r''=a^2\mathbf r'/s^2$. If $|\mathbf r|=a$, expansion of squared [Euclidean distances](../../../../../../euclidean-distance.md) gives

$$
|\mathbf r-\mathbf r''|^2=\frac{a^2}{s^2}|\mathbf r-\mathbf r'|^2.
$$

Consequently $|\mathbf r-\mathbf r''|=(a/s)|\mathbf r-\mathbf r'|$, and the two terms in $H$ cancel. This [method of images](../../../../../../method-of-images.md) gives the [Dirichlet Green function inside a sphere](../../../../../../dirichlet-green-function-inside-a-sphere.md):

$$
\boxed{H(\mathbf r,\mathbf r')=-\frac1{4\pi}\left[\frac1{|\mathbf r-\mathbf r'|}-\frac{a/s}{|\mathbf r-\mathbf r''|}\right].}
$$

The image point is outside the sphere, so only the physical source contributes a [Dirac delta distribution](../../../../../../dirac-delta-function.md) inside. As $s\to0$, the image position tends to infinity and its coefficient also diverges, but their ratio has the finite limit

$$
\frac{a/s}{|\mathbf r-\mathbf r''|}\longrightarrow\frac1a.
$$

Thus

$$
\boxed{H(\mathbf r,0)=-\frac1{4\pi|\mathbf r|}+\frac1{4\pi a}.}
$$

The apparent singularity of the image construction at a central source is removable; the physical source singularity at $\mathbf r=0$ remains.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
