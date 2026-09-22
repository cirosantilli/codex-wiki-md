<h1 id="19/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Lagrange multiplier](../../../../../../lagrange-multiplier.md) condition $\nabla f=\lambda\nabla g$ for $g=4x^2+y^2/16$:

$$
y=8\lambda x,\qquad x=\lambda y/8,\qquad4x^2+y^2/16=1.
$$

Neither coordinate can vanish at a constrained [stationary point](../../../../../../stationary-point.md): either would force both to vanish, contradicting the constraint. Substitution therefore gives $\lambda^2=1$, so $y=8x$ or $y=-8x$. In either case $8x^2=1$, giving

$$
\boxed{(x,y)=\left(\frac{\varepsilon}{2\sqrt2},\ 2\sqrt2\,\delta\right),\qquad
\varepsilon,\delta\in\{-1,1\},\qquad f=\varepsilon\delta}.
$$

Equal signs give the two points attaining the [global maximum](../../../../../../global-maximum.md) $f=1$; opposite signs give the two [global minima](../../../../../../global-minimum.md) with $f=-1$. These exhaust the extrema because the [ellipse](../../../../../../ellipse.md) is compact, its constraint [gradient](../../../../../../gradient.md) never vanishes on it, and $f$ is smooth. The bound can also be checked by setting $X=2x$, $Y=y/4$: then $X^2+Y^2=1$ and $f=2XY$, so $|f|\leq1$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [19](../../../19.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
