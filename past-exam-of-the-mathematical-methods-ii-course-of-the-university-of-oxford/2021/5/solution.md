<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Interpret the cube root as the real cube root. The curved boundary is $y=-x^3$, so the bounded region is $0\le x\le3$, $-x^3\le y\le0$. In particular $y$ is negative inside it. The [double integral](../../../double-integral.md) is the convergent [improper integral](../../../improper-integral.md)

$$
I=\int_0^3\frac1{x^3+1}\left(\int_{-x^3}^0y^{-1/3}\,dy\right)dx.
$$

For negative real $y$, an [antiderivative](../../../antiderivative.md) is $(3/2)y^{2/3}=(3/2)|y|^{2/3}$. The inner [integral](../../../integral-split.md) is therefore $-3x^2/2$. Hence

$$
I=-\frac32\int_0^3\frac{x^2}{x^3+1}\,dx
=-\frac12\bigl[\ln(x^3+1)\bigr]_0^3,
\qquad \boxed{I=-\frac12\ln28.}
$$

The negative sign is essential. Absolute convergence follows by the same calculation with the sign removed, so the singular edge at $y=0$ causes no ambiguity.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2021](../../2021-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
