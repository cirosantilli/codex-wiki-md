<h1 id="differential-equations/8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The lower formula has a smooth continuation as a function of $(x,y)$, and on $y=0$ it has trace $u(x,0)=0$. Its second tangential derivative is

$$
u_{xx}(x,y)=2\pi^2\cos(\pi x)\sin(\pi y),
$$

which vanishes at $y=0$. Hence the continued lower formula satisfies the equation restricted to the interface, where the formal equation is $u_{xx}=0$.

Assuming the solution itself is continuous across the interface, the upper region therefore has the [Dirichlet boundary value problem](../../../../../dirichlet-problem.md)

$$
\boxed{\begin{gathered}
u_{xx}+u_{yy}=0\quad(-1<x<1,\ 0<y<1),\\
u(-1,y)=u(1,y)=0,\qquad u(x,1)=u(x,0)=0.
\end{gathered}}
$$

The zero function satisfies these data. The [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md), applied to both $u$ and $-u$, proves uniqueness among harmonic functions continuous on the closed rectangle. Thus $\boxed{u=0\text{ for }y\geq0}$ is the continuous upper continuation. Satisfaction of the degenerate interface equation does not impose continuity of the normal derivative; that is the issue in part (d).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [Differential Equations](../../../differential-equations.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
