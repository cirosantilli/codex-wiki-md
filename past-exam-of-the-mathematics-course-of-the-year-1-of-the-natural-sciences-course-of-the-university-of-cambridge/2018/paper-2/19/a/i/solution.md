<h1 id="19/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $h=x^2+y^2+z-x$. Using [Lagrange multipliers](../../../../../../lagrange-multiplier.md) with $\nabla f=\lambda\nabla h$ gives

$$
ay=\lambda(2x-1),\qquad ax=2\lambda y,\qquad1=\lambda.
$$

The third equation fixes $\lambda=1$. The first two then reduce to $2x-ay=1$ and $2y=ax$. If $a^2\ne4$, their solution and the constraint give

$$
\boxed{x=\frac2{4-a^2},\qquad y=\frac a{4-a^2},\qquad
z=\frac{4-3a^2}{(4-a^2)^2}.}
$$

At $a=2$, the second equation requires $y=x$ and makes the first inconsistent; at $a=-2$, it requires $y=-x$ and gives the same inconsistency. Thus **there is no constrained stationary point when $a=\pm2$**. The constraint [gradient](../../../../../../gradient.md) never vanishes because its vertical component is one, so the multiplier condition has not excluded any regular constrained [stationary points](../../../../../../stationary-point.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [19](../../../19.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
