<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The original [differential equation](../../../../../differential-equation-split.md) is defined only where $x\ne0$ and $y\ne0$. Put $w=y^3$, so the [chain rule](../../../../../chain-rule.md) gives $w'=3y^2y'$. Multiplying the equation by $3y^2$ yields a first-order [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md):

$$
w'=2x^2+\frac wx,\qquad w'-\frac wx=2x^2.
$$

An [integrating factor](../../../../../integrating-factor.md) on either half-line is $1/x$, up to an irrelevant nonzero constant. Equivalently, apply the [quotient rule](../../../../../quotient-rule.md) directly:

$$
\left(\frac wx\right)'=\frac{w'-w/x}{x}=2x.
$$

Integrating gives $w/x=x^2+C$. Thus the real [general solution](../../../../../general-solution.md) is

$$
\boxed{y(x)=\sqrt[3]{x^3+Cx},\qquad C\in\mathbb R,}
$$

on any connected interval where $x\ne0$ and $x^3+Cx\ne0$. These restrictions preserve both the original denominator and differentiability of the real cube root. In particular $C=0$ includes $y=x$ on either half-line; this solution has not been lost through division by an expression involving $y/x-1$.

For verification, differentiating $y^3=x^3+Cx$ gives $3y^2y'=3x^2+C$, while $(2x^3+y^3)/x=3x^2+C$. The two sides agree wherever the original equation is defined.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
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
