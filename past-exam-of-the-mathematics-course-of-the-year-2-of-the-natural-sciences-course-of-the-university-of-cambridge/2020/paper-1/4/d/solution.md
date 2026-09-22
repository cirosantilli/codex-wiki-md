<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With $c=-b$, equate coefficients in

$$
x(1-x)A''+(1-x)A'+A+2c(1-x)=0.
$$

The constant term is $a_1+2c=0$, and the coefficient of $x$ is $4a_2-2c=0$. Hence

$$
\boxed{a_1=2b,\qquad a_2=-\frac b2.}
$$

For the coefficient of $x^{n-1}$ with $n\geq3$, the first two positive [derivative](../../../../../derivative.md) terms contribute $n^2a_n$, while the remaining analytic terms contribute $[1-(n-1)^2]a_{n-1}$. Thus

$$
\boxed{a_n=\frac{n-2}{n}a_{n-1},\quad n\geq3.}
$$

Iteration gives $a_n=-b/[n(n-1)]$ for $n\geq2$. Using

$$
\sum_{n=2}^\infty\frac{x^n}{n(n-1)}=x+(1-x)\ln(1-x),\qquad |x|<1,
$$

the prescribed solution sums to

$$
\boxed{y=b\left[x+(1-x)\ln\frac{x}{1-x}\right].}
$$

The ansatz starts its analytic [series](../../../../../series-mathematics.md) at $n=1$, so it omits the freedom to add an arbitrary multiple of $1-x$. The complete two-constant real solution on $0<x<1$ is therefore

$$
\boxed{y=C(1-x)+b\left[x+(1-x)\ln\frac{x}{1-x}\right].}
$$

The narrower ansatz in (c) is a convenient choice of the logarithmic solution, not the full [general solution](../../../../../general-solution.md) by itself.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
