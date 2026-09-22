<h1 id="analysis/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For $y''+p(x)y'+q(x)y=0$, a singular point at [zero](../../../../zero-of-a-function.md) is regular when $xp(x)$ and $x^2q(x)$ extend analytically to [zero](../../../../zero-of-a-function.md). Here

$$
p(x)=\frac{\lambda-x}{x(1-x)},\qquad q(x)=\frac1{x(1-x)},
$$

so these products are analytic at [zero](../../../../zero-of-a-function.md). The equation remains singular there because $q$ has a pole.

Substitute $y=\sum_{n\geq0}a_nx^{n+\sigma}$. The lowest power gives the [indicial equation](../../../../indicial-equation.md) $\sigma(\sigma-1+\lambda)=0$. Comparing the next powers gives

$$
\boxed{\sigma=0\text{ or }1-\lambda,\qquad a_{n+1}=\frac{(n+\sigma)^2-1}{(n+\sigma+1)(n+\sigma+\lambda)}a_n.}
$$

For $0<\lambda<1$ the denominators do not vanish. With $\sigma=0$, $a_1=-a_0/\lambda$ and $a_2=0$, so

$$
y_1=a_0(1-x/\lambda),\qquad\boxed{R_1=\infty.}
$$

With $\sigma=1-\lambda$, the recurrence becomes

$$
a_{n+1}=\frac{(n-\lambda)(n+2-\lambda)}{(n+2-\lambda)(n+1)}a_n=\frac{n-\lambda}{n+1}a_n.
$$

Consequently $y_2=a_0x^{1-\lambda}(1-x)^\lambda$ on $0<x<1$, with the [binomial series](../../../../binomial-series.md) for its last factor. The nonzero coefficient ratios tend to one, giving **radius one for that power-series factor**. The factor $x^{1-\lambda}$ specifies the Frobenius branch; the different leading powers prove independence.

When $\lambda=1$, both indicial roots become [zero](../../../../zero-of-a-function.md) and the analytic Frobenius solution in both cases is a multiple of $1-x$. To obtain the missing solution use [reduction of order](../../../../reduction-of-order.md). Away from [zero](../../../../zero-of-a-function.md) and one, $p=1/x$, hence

$$
y_2=(1-x)\int\frac{dx}{x(1-x)^2}=1+(1-x)\log\left|\frac{x}{1-x}\right|.
$$

Thus the real general solution on any interval avoiding the singular points is

$$
\boxed{y=C_1(1-x)+C_2\left[1+(1-x)\log\left|\frac{x}{1-x}\right|\right].}
$$

Its [Wronskian](../../../../wronskian.md) with $1-x$ is $1/x\ne0$, proving independence. For complex solutions choose a logarithm branch on a suitable simply connected region.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Analysis](../../analysis.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
