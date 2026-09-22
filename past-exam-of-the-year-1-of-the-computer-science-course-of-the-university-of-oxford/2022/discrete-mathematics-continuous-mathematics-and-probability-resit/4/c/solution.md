<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $F=x^6+\tfrac32y^4$ and $G=x^4-2y^2-3$. Every [feasible point](../../../../../feasible-point.md) has $x\ne0$, so $\nabla G=(4x^3,-4y)$ cannot vanish. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations are

$$
6x^5=4\lambda x^3,\qquad6y^3=-4\lambda y.
$$

The first gives $\lambda=\tfrac32x^2>0$. If $y\ne0$, the second would give $\lambda=-\tfrac32y^2<0$, a contradiction. Therefore $y=0$, and the [constraint](../../../../../constraint-mechanics.md) gives $x^4=3$. The only constrained [stationary points](../../../../../stationary-point.md) are $(\pm3^{1/4},0)$.

For a global certificate, feasibility implies $x^4\geq3$, and hence

$$
F=(x^4)^{3/2}+\tfrac32y^4\geq3^{3/2}.
$$

Equality requires $y=0$ and $x^4=3$. Thus

$$
\boxed{\min F=3\sqrt3,\qquad (x,y)=(\pm3^{1/4},0).}
$$

The case split is essential: dividing by $y$ would discard precisely the minimizers.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
