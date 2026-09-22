<h1 id="13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the first-order [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md), seek an [integrating factor](../../../../../integrating-factor.md) $M(x)$ that makes its left side a [product rule](../../../../../product-rule.md) [derivative](../../../../../derivative.md). Multiplying by $M$ gives $My'+MPy$, and comparison with $(My)'=My'+M'y$ requires $M'=PM$. On an interval where $P$ is continuous choose

$$
M(x)=\exp\!\left(\int_{x_0}^xP(t)\,dt\right),\qquad M(x_0)=1.
$$

This factor is never zero. The transformed equation is $(My)'=MQ$, so integration from $x_0$ to $x$ yields

$$
\boxed{y(x)=\frac{1}{M(x)}\left[C+\int_{x_0}^x M(t)Q(t)\,dt\right].}
$$

Here $C=y(x_0)$ for an [initial value problem](../../../../../initial-value-problem.md). The [indefinite integral](../../../../../antiderivative.md) version is $y=e^{-\int Pdx}[C+\int Qe^{\int Pdx}dx]$, with any constant choices inside the [integrating factor](../../../../../integrating-factor.md) absorbed into $C$. Continuity of $P,Q$ is a convenient sufficient hypothesis for a classical differentiable [solution of a differential equation](../../../../../solution-of-a-differential-equation.md).

## ↑ Ancestors (13)

1. [B](../b.md)
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
