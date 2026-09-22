<h1 id="f/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The constraint intersection is nonempty, closed and bounded, hence [compact](../../../../../compact-space.md), so extrema exist. The two constraint gradients are $(x/2,2y,2z)$ and $(1,1,-1)$. If the first were $t$ times the second, the plane condition would give $2t+t/2+t/2=0$, so $t=0$ and all coordinates would vanish, contradicting the ellipsoid equation. Their [rank](../../../../../rank-one-quadratic-form.md) is therefore two at every feasible point, justifying the [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations.

These equations are

$$
(1,2,0)=\lambda(x/2,2y,2z)+\mu(1,1,-1),\quad z=x+y.
$$

Eliminating $\mu$ gives $1=\lambda(5x/2+2y)$ and $2=\lambda(2x+4y)$. The first equation makes $\lambda\ne0$; subtracting twice the first from the second forces $x=0$. Hence $z=y$, and the ellipsoid gives $y=z=\pm1/\sqrt2$. Thus

$$
\boxed{g_{\max}=\sqrt2\text{ at }(0,1/\sqrt2,1/\sqrt2),\qquad
 g_{\min}=-\sqrt2\text{ at }(0,-1/\sqrt2,-1/\sqrt2).}
$$

All candidates were found, and [compactness](../../../../../compact-space.md) ensures they include the extrema.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [F](../../../f.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
