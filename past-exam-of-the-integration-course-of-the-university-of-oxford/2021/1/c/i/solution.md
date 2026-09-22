<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For each nonnegative [integer](../../../../../integer-split.md) $k$, the [change of variables](../../../../../change-of-variables-formula.md) $x=e^{-t}$ gives

$$
\int_0^1|(x\log x)^k|\,dx=\int_0^\infty t^ke^{-(k+1)t}\,dt
=\frac{\Gamma(k+1)}{(k+1)^{k+1}}<\infty.
$$

The [gamma function](../../../../../gamma-function.md) identity $\Gamma(k+1)=k!$ follows by repeated [integration by parts](../../../../../integration-by-parts.md). Since $\log x<0$ on $(0,1)$, the sign of the original integrand is $(-1)^k$, so

$$
\boxed{\int_0^1(x\log x)^k\,dx=\frac{(-1)^kk!}{(k+1)^{k+1}}.}
$$

For $k=0$, the integral is one, consistent with the formula.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
