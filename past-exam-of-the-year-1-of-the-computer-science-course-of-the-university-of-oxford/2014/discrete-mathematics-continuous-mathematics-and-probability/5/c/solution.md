<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The constraint implies $x^2=z^2+1$, so $x\ne0$ and its [gradient](../../../../../gradient.md) $(2x,0,-2z)$ never vanishes on the feasible set. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations $\nabla f=\lambda\nabla g$ give

$$
2x=2\lambda x,\qquad2y=0,\qquad1=-2\lambda z.
$$

Thus $\lambda=1$, $y=0$, $z=-1/2$, and feasibility gives $x=\pm\sqrt5/2$. The two stationary points and their values are

$$
\boxed{\left(\frac{\sqrt5}{2},0,-\frac12\right),\
\left(-\frac{\sqrt5}{2},0,-\frac12\right),\qquad f=\frac34.}
$$

They are both [global minima](../../../../../global-minimum.md). Indeed, on the constraint, [completing the square](../../../../../completing-the-square.md) gives

$$
f=1+z^2+y^2+z=\left(z+\frac12\right)^2+y^2+\frac34.
$$

Equality holds only at the two displayed points. There are no other constrained stationary points, and the objective is unbounded above as $|y|\to\infty$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
