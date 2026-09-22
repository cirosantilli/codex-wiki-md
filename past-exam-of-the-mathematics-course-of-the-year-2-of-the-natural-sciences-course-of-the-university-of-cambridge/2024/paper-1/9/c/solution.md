<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This is an [isoperimetric constraint](../../../../../isoperimetric-constraint.md), imposed on the whole path rather than separately at each time. Introduce a constant [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\lambda$ and replace the variational integrand by $\widetilde f=f+\lambda u$. The modified [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) are

$$
\boxed{\frac d{dt}f_{\dot x}-f_x-\lambda u_x=0,\qquad\frac d{dt}f_{\dot y}-f_y-\lambda u_y=0.}
$$

Solve these together with the fixed endpoint conditions, treating $\lambda$ as an unknown constant, then choose its value so that

$$
\boxed{\int_0^Tu(x(t),y(t))\,dt=0.}
$$

The multiplier is constant because there is one scalar [integral](../../../../../integral-split.md) constraint. A condition imposed at every time would instead call for a time-dependent multiplier. As usual, this multiplier procedure assumes the constraint is regular, so its [first variation](../../../../../first-variation.md) does not vanish identically on all admissible [variations](../../../../../variation.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [9](../../9.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
