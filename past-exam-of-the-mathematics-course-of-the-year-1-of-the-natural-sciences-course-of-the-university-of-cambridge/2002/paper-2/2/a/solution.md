<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $F(a)$ be the given [integral](../../../../../integral-split.md). Its integrand extends continuously to $x=0$, with value $a$. The [Leibniz integral rule](../../../../../leibniz-integral-rule.md) includes both the moving upper endpoint and the [derivative](../../../../../derivative.md) of the integrand. For $a\ne0$ it gives

$$
F'(a)=2a\frac{\sin(a\cdot a^2)}{a^2}+\int_0^{a^2}\cos(ax)\,dx=\frac{2\sin(a^3)}a+\frac{\sin(a^3)}a.
$$

Consequently

$$
\boxed{F'(a)=\begin{cases}3\sin(a^3)/a,&a\ne0,\\0,&a=0.\end{cases}}
$$

The zero case follows directly from $F(a)=a^3+O(a^9)$ near zero: expand $\sin(ax)/x=a+O(a^3x^2)$ and integrate up to $a^2$. Equivalently, the [change of variables](../../../../../change-of-variables-formula.md) $t=ax$ gives $F(a)=\int_0^{a^3}(\sin t)/t\,dt$, whose [derivative](../../../../../derivative.md) is the same expression, interpreted continuously at zero. This substitution works for negative $a$ as an oriented [integral](../../../../../integral-split.md) too.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
