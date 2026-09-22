<h1 id="21h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $U=\sum_i u_i$. The candidate strategies are

$$
\boxed{x_i^*=X\frac{u_i}{U},\qquad y_i^*=Y\frac{u_i}{U}.}
$$

At this pair, A's partial derivatives $2u_iy_i/(x_i+y_i)^2$ are independent of $i$, as are the negatives of B's partial derivatives. Since $F$ is concave in $x$ for fixed $y$ and convex in $y$ for fixed $x$, the [Lagrange sufficiency theorem](../../../../../../lagrange-sufficiency-theorem.md) proves

$$
F(x,y^*)\leq F(x^*,y^*)\leq F(x^*,y)
$$

for all feasible $x,y$. Hence $(x^*,y^*)$ is a [saddle point](../../../../../../saddle-point.md) and gives the optimal strategies in this [zero-sum game](../../../../../../zero-sum-game.md). Its game value is

$$
\boxed{F(x^*,y^*)=U\frac{X-Y}{X+Y}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [21H](../../21h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
