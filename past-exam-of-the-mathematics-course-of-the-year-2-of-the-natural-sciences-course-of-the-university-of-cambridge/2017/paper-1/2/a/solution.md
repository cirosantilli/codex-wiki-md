<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $v=(t+1)^2u$, the derivatives are

$$
v_t=2(t+1)u+(t+1)^2u_t,\qquad v_{xx}=(t+1)^2u_{xx}.
$$

Substitution cancels the two terms $2(t+1)u$, giving the [diffusion equation](../../../../../diffusion-equation-split.md)

$$
\boxed{u_t=u_{xx},\qquad u(0,t)=0,\quad u(\pi,t)=\frac{f(t)}{(t+1)^2},\quad u(x,0)=h(x).}
$$

This is a [scalar integrating factor for a reaction-diffusion equation](../../../../../scalar-integrating-factor-for-a-reaction-diffusion-equation.md), since $\exp[\int2\,dt/(t+1)]=(t+1)^2$ up to a constant. We use $t\geq0$, so the factor never vanishes. A classical solution at the initial corners additionally requires compatible data, $h(0)=0$ and $h(\pi)=f(0)$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
