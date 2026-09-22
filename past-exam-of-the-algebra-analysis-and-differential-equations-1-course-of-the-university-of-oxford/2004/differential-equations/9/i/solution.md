<h1 id="differential-equations/9/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

This is the **[heat equation](../../../../../heat-equation.md)**, with $y$ as time. The stated zero solution is **unique**. Define $E(y)=\frac12\int_0^1u(x,y)^2\,dx$. For $0<y<1$, [integration by parts](../../../../../integration-by-parts.md) and $u_y=u_{xx}$ give

$$
E'(y)=\int_0^1u\,u_{xx}\,dx=[uu_x]_0^1-\int_0^1u_x^2\,dx=-\int_0^1u_x^2\,dx\leq0.
$$

The boundary term is zero because $u(0,y)=0$ and $u_x(1,y)=0$. Also $E(0)=0$. Nonnegativity forces $E(y)=0$, and [continuity](../../../../../continuous-function.md) gives $u=0$ throughout the square. The unknown final-time boundary values are determined by evolution and need not be prescribed. Under the stated regularity the integrations can first be made on an interior interval and then passed to the endpoints using [continuity](../../../../../continuous-function.md) of $u,u_x,u_y$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [9](../../9.md)
3. [Differential equations](../../../differential-equations.md)
4. [2004](../../../../2004-split.md)
5. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
