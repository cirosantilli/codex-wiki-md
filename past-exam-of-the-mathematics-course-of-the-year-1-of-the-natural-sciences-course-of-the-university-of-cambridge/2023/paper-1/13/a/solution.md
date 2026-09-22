<h1 id="13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On an [interval](../../../../../interval-mathematics.md) with $x\ne0$, division by $x^2$ gives the [separable differential equation](../../../../../separable-differential-equation.md) $y'=(4/x^2-1/x)y^2$. For $y\ne0$, take [antiderivatives](../../../../../antiderivative.md):

$$
\int\frac{dy}{y^2}=\int\left(\frac4{x^2}-\frac1x\right)dx,\qquad -\frac1y=-\frac4x-\ln|x|+C.
$$

Renaming the constant yields the explicit nonzero family

$$
\boxed{y(x)=\frac1{4/x+\ln|x|+C}.}
$$

For $x\ne0$, the [interval](../../../../../interval-mathematics.md) of definition must avoid zeros of the denominator. Division by $y^2$ excluded the additional solution $\boxed{y(x)\equiv0}$, which must also be included.

The original undivided [differential equation](../../../../../differential-equation-split.md) also makes sense at $x=0$, where it requires $y(0)=0$. For [continuation through a zero of the leading ODE coefficient](../../../../../continuation-through-a-zero-of-the-leading-ode-coefficient.md), rewrite the nonzero family as

$$
y(x)=\frac{x}{4+x\ln|x|+Cx}.
$$

It extends differentiably with $y(0)=0$ and $y'(0)=1/4$, since $y(x)/x\to1/4$. One may choose the integration constants independently on the two sides of zero and obtain a differentiable solution through zero. The zero solution also extends through zero, with [derivative](../../../../../derivative.md) $0$; joining a nonzero branch on just one side to a zero branch on the other would fail [differentiability](../../../../../differentiability.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
