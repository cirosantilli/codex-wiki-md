<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Divide the [Chebyshev differential equation](../../../../../chebyshev-differential-equation.md) by $1-x^2$. Its coefficients $-x/(1-x^2)$ and $m^2/(1-x^2)$ are analytic at zero, so $\boxed{x=0\text{ is an ordinary point}.}$ The finite [singular points of a differential equation](../../../../../singular-point-of-a-differential-equation.md) are $x=\pm1$.

Insert $y=\sum_{n\geq0}a_nx^{n+\sigma}$, $a_0\ne0$. The coefficient of the lowest power $x^{\sigma-2}$ is $\sigma(\sigma-1)a_0$, hence $\sigma=0$ or $1$. The next power gives $\sigma(\sigma+1)a_1=0$, and the remaining powers yield

$$
\boxed{a_{n+2}=\frac{(n+\sigma)^2-m^2}{(n+\sigma+2)(n+\sigma+1)}a_n,\qquad n\geq0.}
$$

For $\sigma=0$, $a_1$ is free and

$$
a_{n+2}=\frac{n^2-m^2}{(n+2)(n+1)}a_n.
$$

Choosing $a_1=0$ selects the even [power series](../../../../../power-series.md), with $y(0)=a_0,y'(0)=0$. For $\sigma=1$, the next-power equation forces $a_1=0$ and

$$
a_{n+2}=\frac{(n+1)^2-m^2}{(n+3)(n+2)}a_n.
$$

This selects the odd [power series](../../../../../power-series.md), with $y(0)=0,y'(0)=a_0$. Their different initial values prove [linear independence](../../../../../linear-independence.md). Although the [Frobenius method](../../../../../frobenius-method.md) produces two possible leading exponents, zero is an [ordinary point](../../../../../ordinary-point-criterion-for-a-second-order-equation.md), and a general $\sigma=0$ series already includes both initial constants.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
