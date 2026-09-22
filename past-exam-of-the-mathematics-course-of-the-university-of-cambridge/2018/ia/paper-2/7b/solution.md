<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

After division by $x^2$, the equation is $y''+x^{-1}y'-(1+\alpha^2x^{-2})y=0$. Every $x\ne0$ is an [ordinary point](../../../../../ordinary-point-criterion-for-a-second-order-equation.md). The origin is singular, but it is a [regular singular point](../../../../../regular-singular-point.md) because $xP(x)=1$ and $x^2Q(x)=-(x^2+\alpha^2)$ are analytic there. An ordinary point has analytic normalized coefficients $P,Q$; a singular point failing the displayed regularity test is irregular.

The [Frobenius method](../../../../../frobenius-method.md) ansatz $y=x^r\sum_{n\geq0}a_nx^n$ gives the indicial equation $r^2-\alpha^2=0$, $a_1=0$, and

$$
a_n=\frac{a_{n-2}}{(n+r)^2-\alpha^2}.
$$

For nonintegral $\alpha$, two independent solutions are

$$
\boxed{\begin{aligned}
y_+&=x^\alpha\left(1+\frac{x^2}{4(\alpha+1)}
+\frac{x^4}{32(\alpha+1)(\alpha+2)}+\cdots\right),\\
y_-&=x^{-\alpha}\left(1+\frac{x^2}{4(1-\alpha)}
+\frac{x^4}{32(1-\alpha)(2-\alpha)}+\cdots\right).
\end{aligned}}
$$

For integral $\alpha$, put $m=|\alpha|$. In the $r=-m$ recurrence the denominator vanishes at $n=2m$, so that series fails or coincides in the exceptional $m=0$ case. Up to scale the single Frobenius series is

$$
\boxed{y_1=x^m\left(1+\frac{x^2}{4(m+1)}
+\frac{x^4}{32(m+1)(m+2)}+\cdots\right),\quad
a_{2k}=\frac{a_{2k-2}}{4k(m+k)}.}
$$

For $\alpha=1$, $y_1=x(1+x^2/8+\cdots)$, so

$$
\frac1{s\,y_1(s)^2}=s^{-3}-\frac1{4s}+O(s).
$$

Its integral contains both $s^{-2}$ and $\log s$; multiplying by $y_1$ leaves a pole and a logarithmic term. Thus the reduction-of-order solution is not a power series at zero.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
