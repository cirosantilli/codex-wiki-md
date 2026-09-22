<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The continuous [function](../../../../../function-split.md) attains a global maximum and minimum on the closed disc by the [extreme value theorem](../../../../../extreme-value-theorem.md). All four unconstrained [stationary points](../../../../../stationary-point.md) have squared distance eight, so none lies in its interior. The extrema must therefore lie on $x^2+y^2=6$.

The constraint [gradient](../../../../../gradient.md) is nonzero on that circle, so [Lagrange multipliers](../../../../../lagrange-multiplier.md) apply:

$$
\frac{x^2}4-1=2\lambda x,\qquad\frac{y^2}4-1=2\lambda y.
$$

Subtracting gives $(x-y)((x+y)/4-2\lambda)=0$. If $x=y$, the constraint gives $x=y=\pm\sqrt3$. Otherwise $2\lambda=(x+y)/4$; substitution into either equation gives $xy=-4$. This is impossible, since $|xy|\leq(x^2+y^2)/2=3$ on the circle. Thus the diagonal points are the only candidates. Comparing their values gives

$$
\boxed{\min f=-\frac{3\sqrt3}{2}\text{ at }(\sqrt3,\sqrt3),\qquad\max f=\frac{3\sqrt3}{2}\text{ at }(-\sqrt3,-\sqrt3).}
$$

## ↑ Ancestors (12)

1. [F](../f.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
