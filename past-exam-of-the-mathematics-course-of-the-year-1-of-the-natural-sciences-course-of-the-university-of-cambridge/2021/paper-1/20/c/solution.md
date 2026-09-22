<h1 id="20/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First check the [improper integral](../../../../../improper-integral.md) exists: near zero its numerator is $(\beta-\alpha)x^2+O(x^4)$, so the quotient is $O(x)$; at infinity both exponentials decay. For positive parameters in compact neighborhoods, the differentiated integrands have integrable bounds, justifying [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md). It gives

$$
\frac{\partial I}{\partial\alpha}=-\int_0^\infty xe^{-\alpha x^2}\,dx=-\frac1{2\alpha},\qquad\frac{\partial I}{\partial\beta}=\int_0^\infty xe^{-\beta x^2}\,dx=\frac1{2\beta}.
$$

Thus $I=-\tfrac12\ln\alpha+\tfrac12\ln\beta+C$, with $C$ independent of both parameters. Since $I(\alpha,\alpha)=0$, $C=0$, and

$$
\boxed{I(\alpha,\beta)=\frac12\ln\frac\beta\alpha.}
$$

The sign is consistent with the integrand: $\beta>\alpha$ makes it positive. Neither separate integral $\int_0^\infty e^{-\alpha x^2}\,dx/x$ converges at zero; it is the difference that is meaningful. The substitution $u=x^2$ identifies the result as a [Frullani integral](../../../../../frullani-integral.md) with an extra factor $1/2$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
