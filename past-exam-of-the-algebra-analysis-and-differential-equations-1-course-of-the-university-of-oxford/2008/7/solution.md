<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Rewrite the linear equation as $(x^2y)'=0$. The initial value gives the unique solution

$$
\boxed{y(x)=x^{-2}\quad(x>0).}
$$

The [Picard iteration](../../../picard-iteration.md) is its integral equation

$$
y_{n+1}(x)=1-2\int_1^x\frac{y_n(t)}t\,dt.
$$

The proposed formula holds for $n=0$. If it holds at $n$, termwise integration of the finite sum and $d(\log t)/dt=1/t$ give

$$
y_{n+1}(x)
=1+\sum_{k=0}^n\frac{(-2\log x)^{k+1}}{(k+1)!}
=\sum_{k=0}^{n+1}\frac{(-2\log x)^k}{k!}.
$$

This proves the expression by induction. The [exponential series](../../../exponential-series.md) then gives $y_n(x)\to e^{-2\log x}=x^{-2}$. Convergence is also uniform on every compact subinterval of $(0,\infty)$, since $|\log x|$ is bounded there and the exponential majorant series converges. This is [Picard iteration for a simple-pole linear differential equation](../../../picard-iteration-for-a-simple-pole-linear-differential-equation.md).

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2008](../../2008-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
