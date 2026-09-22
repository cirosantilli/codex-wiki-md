<h1 id="19/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The base lies in the plane $z=R-h$. Its circular rim lies on the [sphere](../../../../../sphere.md), so

$$
r^2+(R-h)^2=R^2,\qquad 0\leq h\leq2R.
$$

Maximize the [cone](../../../../../cone-geometry.md) volume $V_c=\pi r^2h/3$ using the [Lagrange multiplier](../../../../../lagrange-multiplier.md) expression

$$
\mathcal L=\frac\pi3r^2h-\lambda\bigl[r^2+(R-h)^2-R^2\bigr].
$$

For a nondegenerate [cone](../../../../../cone-geometry.md), the $r$ equation gives $\lambda=\pi h/3$. The $h$ equation is $\pi r^2/3+2\lambda(R-h)=0$, hence $r^2=2h(h-R)$. Combining this with $r^2=2Rh-h^2$ gives

$$
\boxed{h=\frac{4R}{3},\qquad r=\frac{2\sqrt2}{3}R}.
$$

Indeed, eliminating $r$ gives $V_c(h)=\pi h^2(2R-h)/3$, which vanishes at the endpoints and has a unique positive interior maximum at $4R/3$. Thus

$$
\boxed{V_{c,\max}=\frac{32\pi R^3}{81},\qquad
\frac{V_{c,\max}}{(4/3)\pi R^3}=\frac8{27}}.
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [19](../../19.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
