<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Lagrangian](../../../../../lagrangian.md)

$$
\mathcal L=x^4+4y^4-\lambda(x^2-y^2-1).
$$

The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations are

$$
4x^3-2\lambda x=0,\qquad
16y^3+2\lambda y=0,\qquad x^2-y^2=1.
$$

Feasibility makes $x\ne0$, so $\lambda=2x^2>0$. The second equation becomes $2y(8y^2+\lambda)=0$, forcing $y=0$ and then $x=\pm1$. The constraint [gradient](../../../../../gradient.md) $(2x,-2y)$ is nonzero on the feasible set, so the multiplier calculation has no missing singular feasible point.

To verify the global minimum rather than just stationarity, eliminate $x^2=1+y^2$:

$$
x^4+4y^4=1+2y^2+5y^4\ge1.
$$

Equality holds exactly at **$(x,y)=(1,0)$ or $(-1,0)$, with minimum value $1$**.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
