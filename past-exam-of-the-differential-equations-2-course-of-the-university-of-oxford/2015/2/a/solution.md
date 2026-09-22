<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Divide by $2x$ away from zero to obtain $y''+P(x)y'+Q(x)y=0$, with $P(x)=x/2-1/(2x)$ and $Q(x)=\lambda/2$. At zero, the quantities $xP(x)=(x^2-1)/2$ and $x^2Q(x)=\lambda x^2/2$ are analytic. The [pole](../../../../pole.md) in $P$ makes zero singular, so **$x=0$ is a [regular singular point](../../../../regular-singular-point.md)**. Its [indicial equation](../../../../indicial-equation.md) is

$$
r(r-1)+\left(-\frac12\right)r+0=0,
\qquad\boxed{r_1=0,\quad r_2=\frac32.}
$$

At $x=1$, both normalized [coefficients](../../../../coefficient.md) are analytic [functions](../../../../function-split.md), so **$x=1$ is an [ordinary point](../../../../ordinary-point-criterion-for-a-second-order-equation.md)**. These are the standard normalized-[coefficient](../../../../coefficient.md) and indicial tests.[§2.7(i), equations 2.7.1–2.7.3](../../../../nist-digital-library-of-mathematical-functions.md)

For infinity, set $t=1/x$ and $Y(t)=y(1/t)$. The [chain rule](../../../../chain-rule.md) gives $y'=-t^2Y'$ and $y''=t^4Y''+2t^3Y'$, so the transformed normalized equation is

$$
Y''+\left(\frac5{2t}-\frac1{2t^3}\right)Y'+\frac\lambda{2t^4}Y=0.
$$

The product of the first-[derivative](../../../../derivative.md) [coefficient](../../../../coefficient.md) with $t$ still has a second-order [pole](../../../../pole.md) at zero. Hence the criterion for a [regular singular point](../../../../regular-singular-point.md) fails and **$x=\infty$ is an [irregular singular point](../../../../irregular-singular-point.md)**, including when $\lambda=0$. The primes on $Y$ here refer to [differentiation](../../../../differentiation.md) with respect to $t$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
