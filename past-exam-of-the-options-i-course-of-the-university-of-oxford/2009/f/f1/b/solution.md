<h1 id="f/f1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use constraints $h_1=x^2/4+y^2+z^2-1$ and $h_2=x+y-z$. Both constraints and the objective are [continuously differentiable](../../../../../continuously-differentiable-function.md). The feasible set is a nonempty [closed subset](../../../../../closed-set.md) of a bounded ellipsoid, hence [compact](../../../../../compact-space.md), so the [extreme value theorem](../../../../../extreme-value-theorem.md) guarantees both extrema.

The gradients $(x/2,2y,2z)$ and $(1,1,-1)$ are independent everywhere feasible. If the first were $t$ times the second, then $x=2t$, $y=t/2$, $z=-t/2$. The plane constraint would give $3t=0$, forcing the origin, which is not on the ellipsoid. Thus the [Lagrange multiplier](../../../../../lagrange-multiplier.md) theorem applies at every feasible point.

Its equations are

$$
1=\lambda x/2+\mu,\qquad
2=2\lambda y+\mu,\qquad
0=2\lambda z-\mu.
$$

Here $\lambda\ne0$, since otherwise the first two equations require $\mu=1=2$. Subtract twice the first equation from the second, and use $\mu=2\lambda z$ and $z=x+y$; the result is $0=-3\lambda x$, so $x=0$. Then $z=y$ and the ellipsoid gives $y=\pm1/\sqrt2$. The only candidates are therefore $(0,\pm1/\sqrt2,\pm1/\sqrt2)$, with matching signs. Consequently

$$
\boxed{\min g=-\sqrt2,\qquad\max g=\sqrt2}.
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [F1](../../f1.md)
3. [F](../../../f.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
