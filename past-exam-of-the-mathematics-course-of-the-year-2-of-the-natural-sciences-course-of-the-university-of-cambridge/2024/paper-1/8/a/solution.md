<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First simplify the coefficient of $y$ using

$$
\frac{m^3}{x-m}+x^2+mx+m^2=\frac{x^3}{x-m}.
$$

After dividing by $x(x-m)$, the [second-order linear differential equation](../../../../../second-order-linear-differential-equation.md) is

$$
y''+P(x)y'+Q(x)y=0,\qquad P(x)=\frac1x+\frac1{x-m},\qquad Q(x)=\frac{\omega^2x^2}{(x-m)^2}.
$$

At zero, $xP\to1$ and $x^2Q\to0$, and both products are analytic there. At $m$, $(x-m)P\to1$ and $(x-m)^2Q\to m^2\omega^2$, again with analytic extensions. Thus $\boxed{x=0\text{ and }x=m\text{ are regular singular points}}$, and there are no other finite singular points.

Infinity must also be considered because the question asks for all singular points. Put $t=1/x$ and $Y(t)=y(1/t)$. The coefficient of $Y$ in its normal-form equation is $Q(1/t)/t^4\sim\omega^2/t^4$. Multiplication by $t^2$ does not make it analytic at zero. Hence $\boxed{x=\infty\text{ is an irregular singular point}}$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
