<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose $u=x-y$ and $v=x+y$. Then $0\le u\le1$, $1\le v\le3$, while $x=(v+u)/2$, $y=(v-u)/2$ and the inverse [Jacobian determinant](../../../../jacobian-determinant.md) has magnitude $1/2$. Hence

$$
\iint_R\left(\frac{x-y}{x+y+3}\right)^2\,dx\,dy
=\frac12\int_0^1u^2\,du\int_1^3(v+3)^{-2}\,dv
=\frac16\left(\frac14-\frac16\right)
=\boxed{\frac1{72}.}
$$

The denominator is bounded away from zero on the transformed rectangle, so no singularity or improper-integral qualification is needed.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2016 resit](../../../2016-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
