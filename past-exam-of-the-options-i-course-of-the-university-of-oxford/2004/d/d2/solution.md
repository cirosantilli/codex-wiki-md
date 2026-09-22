<h1 id="d/d2/solution">Solution</h1>

↑ **Parent:** [D2](../d2.md)

The indicated [measurable function](../../../../measurable-function.md) is nonnegative. [Tonelli's theorem](../../../../tonelli-theorem.md) applies without first assuming [integrability](../../../../integrability.md) and gives

$$
\int_{\mathbb R^2}h=\int_a^b\left(\int_1^\infty x^{-y}\,dx\right)dy
=\int_a^b\frac{dy}{y-1}=\log\frac{b-1}{a-1}<\infty.
$$

Thus $h$ is integrable. [Fubini's theorem](../../../../fubini-s-theorem.md) now allows the reverse order. For $x>1$,

$$
\int_a^bx^{-y}\,dy=\frac{x^{-a}-x^{-b}}{\log x}.
$$

Consequently

$$
\boxed{\int_1^\infty\frac{x^{-a}-x^{-b}}{\log x}\,dx=\log\frac{b-1}{a-1}.}
$$

At $x=1$ the quotient has the removable limit $b-a$; that endpoint does not create an additional divergence.

## ↑ Ancestors (12)

1. [D2](../d2.md)
2. [D](../../d.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
