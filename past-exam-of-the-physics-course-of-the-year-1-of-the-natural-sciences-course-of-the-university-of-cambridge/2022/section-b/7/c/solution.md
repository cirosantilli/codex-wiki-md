<h1 id="section-b/7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $s=r_0+\mu t$. The proposed [velocity](../../../../../velocity.md) and its [derivative](../../../../../derivative.md) are

$$
v=\frac{g}{4\mu}\left(s-\frac{r_0^4}{s^3}\right),\qquad\dot v=\frac g4\left(1+\frac{3r_0^4}{s^4}\right).
$$

The remaining term in the [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md) is

$$
\frac{3\mu}{s}v=\frac{3g}{4}\left(1-\frac{r_0^4}{s^4}\right),
$$

so the sum is exactly $g$. Also $v(0)=g(r_0-r_0)/(4\mu)=0$, establishing both the equation and its [initial condition](../../../../../initial-condition.md):

$$
\boxed{v(t)=\frac g{4\mu}\left[(r_0+\mu t)-\frac{r_0^4}{(r_0+\mu t)^3}\right].}
$$

The [integrating factor](../../../../../integrating-factor.md) $(r_0+\mu t)^3$ explains where the expression comes from:

$$
\frac d{dt}(s^3v)=gs^3,\qquad s^3v=\frac{g}{4\mu}(s^4-r_0^4).
$$

The result has units of [velocity](../../../../../velocity.md). Its continuous $\mu\to0$ limit is $gt$, despite the apparent $1/\mu$ in the written expression.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
