<h1 id="17/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [product substitution for a first-order equation](../../../../../product-substitution-for-a-first-order-equation.md) $v=xy$. The [product rule](../../../../../product-rule.md) gives $v'=xy'+y$, turning the equation into $v'=e^v$. Consequently $(e^{-v})'=-1$, so $e^{-v}=C-x$.

At $x=1$ the initial value gives $v=1$, hence $C=1+e^{-1}$. Recovering $y=v/x$ gives

$$
\boxed{y(x)=-\frac{\ln(1+e^{-1}-x)}{x},\qquad 0<x<1+e^{-1}.}
$$

This is the maximal real graph [interval](../../../../../interval-mathematics.md) containing the initial point: the logarithm requires $x<1+e^{-1}$, and the numerator has a nonzero limit at zero, so this [particular solution](../../../../../particular-solution.md) cannot extend through zero. Differentiating $xy=-\ln(C-x)$ verifies $xy'+y=1/(C-x)=e^{xy}$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
