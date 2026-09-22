<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose the convention $L_xG(x,s)=\delta(x-s)$, where $\delta$ is the [Dirac delta distribution](../../../../../dirac-delta-function.md), together with $G(1/2,s)=G(1,s)=0$. The [Green's function](../../../../../green-s-function-split.md) is continuous at $x=s$ and obeys

$$
\partial_xG(s^+,s)-\partial_xG(s^-,s)=1.
$$

These conditions follow by integrating its [differential equation](../../../../../differential-equation-split.md) across $s$; continuity prevents a derivative of the [Dirac delta distribution](../../../../../dirac-delta-function.md). If $\ell$ and $r$ are homogeneous solutions satisfying the left and right [boundary conditions](../../../../../boundary-condition.md), respectively, and $W=\ell r'-\ell'r$ is their [Wronskian](../../../../../wronskian.md), then

$$
G(x,s)=\frac{\ell(x_<)r(x_>)}{W(s)},\qquad x_<=\min(x,s),\quad x_>=\max(x,s).
$$

For $n\ne0$ take $\ell(x)=x^{-n}-2^n$ and $r(x)=x^{-n}-1$. Their [Wronskian](../../../../../wronskian.md) is $W(s)=n(2^n-1)s^{-n-1}$, and hence

$$
\boxed{G_n(x,s)=\frac{s^{n+1}(x_<^{-n}-2^n)(x_>^{-n}-1)}{n(2^n-1)},\qquad n\ne0.}
$$

For $n=0$ take $\ell(x)=\log(2x)$ and $r(x)=\log x$, giving $W(s)=\log2/s$ and

$$
\boxed{G_0(x,s)=\frac{s}{\log2}\log(2x_<)\log x_>.}
$$

Both formulas satisfy the endpoint conditions, continuity, and the unit jump directly. The unique solution of the [boundary value problem](../../../../../boundary-value-problem-split.md) is

$$
\boxed{u(x)=\int_{1/2}^1G_n(x,s)f(s)\,ds.}
$$

The factor $s^{n+1}$ in the first formula matters: this [Green's function](../../../../../green-s-function-split.md) is for the original monic [differential operator](../../../../../differential-operator.md), with ordinary measure $ds$, rather than for the operator multiplied by $x^{n+1}$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
