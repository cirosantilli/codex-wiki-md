<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Invert the change of variables: $x=(v-u)/2$, $y=(v+u)/2$. The absolute [Jacobian determinant](../../../jacobian-determinant.md) is $1/2$, and the transformed triangle is $0\le v\le3$, $-v\le u\le v$. Hence

$$
I=\frac12\int_0^3\int_{-v}^{v}e^{u/v}\,du\,dv
=\frac12\int_0^3v(e-e^{-1})\,dv
=\boxed{\frac94(e-e^{-1})=\frac92\sinh1.}
$$

At the single vertex $v=0$, the printed integrand is undefined. This causes no integral divergence: throughout the remaining triangle $-1\le u/v\le1$, so the integrand is bounded between $e^{-1}$ and $e$. Giving the vertex any finite value, or taking a limiting integral with $v>0$, gives the same answer.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2017 resit](../../2017-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
