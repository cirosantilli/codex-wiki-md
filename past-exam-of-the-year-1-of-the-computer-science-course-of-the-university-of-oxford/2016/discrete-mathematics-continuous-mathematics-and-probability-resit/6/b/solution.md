<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The constraint is a [compact set](../../../../../compact-space.md), so the continuous objective attains both extrema by the [extreme value theorem](../../../../../extreme-value-theorem.md). Use [Lagrange multipliers](../../../../../lagrange-multiplier.md) with $q(x,y)=9x^2+y^2$:

$$
(4,1)=\lambda(18x,2y).
$$

Since the second component makes $\lambda\ne0$, the two equations give $4/(18x)=1/(2y)$, or $y=9x/4$. Substitution into the constraint yields

$$
\frac{225}{16}x^2=36,\qquad x=\pm\frac85,\quad y=\pm\frac{18}5,
$$

with matching signs. The objective values are therefore

$$
\boxed{\max(4x+y)=10\text{ at }(8/5,18/5),\qquad
\min(4x+y)=-10\text{ at }(-8/5,-18/5)}.
$$

The constraint gradient never vanishes on the ellipse, so these are all the possible extrema. As a direct check, set $u=3x$, $v=y$; then $u^2+v^2=36$ and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $|4u/3+v|\leq6\sqrt{16/9+1}=10$, with equality at the same points.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics and probability (resit)](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
