<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

Write a [power series](../../../../../power-series.md) $y=\sum_{n\geq0}c_nx^n$. Substitution gives

$$
\sum_{n\geq0}n(n-2)c_nx^{n-1}+4\sum_{n\geq0}c_nx^{n+3}=0.
$$

The lowest coefficients give $c_1=0$, $c_3=0$, with $c_0,c_2$ free. For $n\geq4$, matching the coefficient of $x^{n-1}$ gives the recurrence

$$
\boxed{c_n=-\frac{4c_{n-4}}{n(n-2)}.}
$$

All odd coefficients consequently vanish. For the first solution, $c_0=a$, $c_2=y_1''(0)/2=0$, so the first three nonzero terms, when $a\ne0$, are

$$
\boxed{y_1(x)=a-\frac a2x^4+\frac a{24}x^8+O(x^{12}).}
$$

For the second, $c_0=0$, $c_2=b/2$, giving

$$
\boxed{y_2(x)=\frac b2x^2-\frac b{12}x^6+\frac b{240}x^{10}+O(x^{14}).}
$$

If its prescribed constant is zero, the corresponding solution is identically zero and has no nonzero terms.

For the change of variable, put $y(x)=Y(u)$, $u=x^\alpha$, with $\alpha\ne0$. The [chain rule](../../../../../chain-rule.md) gives

$$
xy''-y'+4x^3y
=\alpha^2x^{2\alpha-1}Y_{uu}
+\alpha(\alpha-2)x^{\alpha-1}Y_u+4x^3Y.
$$

After division by $x^{2\alpha-1}$, the coefficient of $Y_u$ is $\alpha(\alpha-2)x^{-\alpha}$ and that of $Y$ is $4x^{4-2\alpha}$. A genuine constant-coefficient equation requires $\alpha=2$, which both removes $Y_u$ and makes the final coefficient constant. The transformed equation is $4Y_{uu}+4Y=0$.

This [quadratic-variable reduction of a singular oscillator](../../../../../quadratic-variable-reduction-of-a-singular-oscillator.md) yields

$$
\boxed{\alpha=2,\qquad y(x)=A\cos(x^2)+B\sin(x^2).}
$$

It holds on each interval away from zero and both solutions extend smoothly through zero. Here $y(0)=A$ and $y''(0)=2B$, so the specified solutions are exactly $a\cos(x^2)$ and $(b/2)\sin(x^2)$. Their [Taylor series](../../../../../taylor-series.md) agree with the recurrences above. Although the original equation has a [regular singular point](../../../../../regular-singular-point.md) at zero, these two [linearly independent](../../../../../linear-independence.md) smooth solutions supply the required data there.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
