<h1 id="13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $1+x^2>0$ for all real $x$, divide the equation by that factor. Its linear coefficient can be integrated by [polynomial division](../../../../../polynomial-division.md):

$$
P(x)=\frac{3x^3}{1+x^2}=3x-\frac{3x}{1+x^2},\qquad
\int P(x)\,dx=\frac32x^2-\frac32\ln(1+x^2).
$$

Thus a positive [integrating factor](../../../../../integrating-factor.md) is $M=e^{3x^2/2}(1+x^2)^{-3/2}$. Multiplying the divided equation gives the [product rule](../../../../../product-rule.md) form

$$
\frac d{dx}(My)=\frac{6x}{(1+x^2)^{5/2}}.
$$

The [integration by substitution](../../../../../integration-by-substitution.md) $u=1+x^2$ gives

$$
My=-\frac{2}{(1+x^2)^{3/2}}+C,\qquad
y=e^{-3x^2/2}\big[C(1+x^2)^{3/2}-2\big].
$$

The [initial condition](../../../../../initial-condition.md) $y(0)=1$ fixes $C-2=1$. The required solution is therefore

$$
\boxed{y(x)=e^{-3x^2/2}\left[3(1+x^2)^{3/2}-2\right],\qquad x\in\mathbb R.}
$$

No real singularity was introduced by the division or the [integrating factor](../../../../../integrating-factor.md), so the solution extends over the entire real line.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
