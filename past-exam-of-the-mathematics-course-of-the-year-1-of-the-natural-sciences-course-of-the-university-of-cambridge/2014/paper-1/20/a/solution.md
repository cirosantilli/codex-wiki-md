<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Maximizing the squared distance avoids differentiating a square root. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations for $f=x^2+y^2$ are

$$
2x=\lambda(2x+y),\qquad2y=\lambda(x+2y),\qquad x^2+y^2+xy=4.
$$

Adding and subtracting the first two gives $(2-3\lambda)(x+y)=0$ and $(2-\lambda)(x-y)=0$. The feasible [stationary points](../../../../../stationary-point.md) therefore lie on $x=y$ or $x=-y$. The first case gives $(x,y)=(\pm2/\sqrt3,\pm2/\sqrt3)$ and squared distance $8/3$. The second gives $(2,-2)$ and $(-2,2)$, with squared distance $8$.

The [ellipse](../../../../../ellipse.md) is compact and its constraint [gradient](../../../../../gradient.md) does not vanish on the curve, so an extremum exists among these points. A direct global check is $4=f+xy\geq f/2$, using $xy\geq-f/2$. Equality occurs when $x=-y$. Consequently

$$
\boxed{d_{\max}=2\sqrt2,\qquad\text{at }(2,-2),\ (-2,2).}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
