<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $|x|<1$, the [geometric series](../../../../geometric-series.md) gives $(1+x)^{-1}=\sum_{j=0}^\infty(-x)^j$. Integrating from zero to $x$ yields the [Maclaurin series](../../../../maclaurin-series.md)

$$
\boxed{\ln(1+x)=\sum_{j=1}^\infty\frac{(-1)^{j+1}x^j}{j}
=x-\frac{x^2}{2}+\frac{x^3}{3}-\cdots.}
$$

On the real axis the series also converges at $x=1$ to $\ln2$, but diverges at $x=-1$.

For fixed real $a$ and sufficiently large positive $x$, the base in the requested limit is positive. Apply the series with argument $-a^2/x^2$:

$$
x^2\ln\left(1-\frac{a^2}{x^2}\right)
=-a^2-\frac{a^4}{2x^2}+O(x^{-4})\longrightarrow-a^2.
$$

Continuity of the [exponential function](../../../../exponential-function.md) therefore gives

$$
\boxed{\lim_{x\to\infty}\left(1-\frac{a^2}{x^2}\right)^{x^2}=e^{-a^2}.}
$$

This includes $a=0$, when the expression is identically one.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2019 resit](../../../2019-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
