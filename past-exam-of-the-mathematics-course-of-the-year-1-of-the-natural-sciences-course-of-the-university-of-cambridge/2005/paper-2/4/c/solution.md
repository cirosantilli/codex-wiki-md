<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $w>0$ denote the stated cost per area of the cylindrical wall. Charge for the curved wall and cap as specified; no floor cost is supplied. The volume and cost are $V=\pi r^2h+2\pi r^3/3$ and $C=2\pi wrh+4\pi wr^2$. To minimize cost at fixed volume, apply a [Lagrange multiplier](../../../../../lagrange-multiplier.md) to $C-\lambda(\pi r^2h+2\pi r^3/3-V)$. Differentiation with respect to $h$ gives $\lambda=2w/r$. The $r$ derivative then gives $2\pi wh+8\pi wr=\lambda(2\pi rh+2\pi r^2)$, reducing to $h=2r$. Thus the [optimal cylinder and hemispherical cap with unequal surface costs](../../../../../optimal-cylinder-and-hemispherical-cap-with-unequal-surface-costs.md) has

$$
\boxed{r=\left(\frac{3V}{8\pi}\right)^{1/3},\qquad h=2\left(\frac{3V}{8\pi}\right)^{1/3}.}
$$

For a global check, eliminate $h$ to obtain $C(r)=2wV/r+(8\pi w/3)r^2$. Its second derivative is positive for $r>0$, and its critical radius gives $h>0$, so the constrained optimum lies inside the physically feasible range and is the unique minimum.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
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
