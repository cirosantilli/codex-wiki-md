<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The given [probability density function](../../../../../probability-density-function.md) is that of a [beta distribution](../../../../../beta-distribution.md) with parameters $r$ and $n-r+1$. We can derive the required [moments](../../../../../moment.md) directly rather than assuming the beta moment formulas. For an integer $j\geq0$, the [Euler beta function](../../../../../beta-function.md) gives

$$
\begin{aligned}
\mathbb E[U_{(r)}^j]
&=\frac{n!}{(r-1)!(n-r)!}
\int_0^1u^{r+j-1}(1-u)^{n-r}\,du\\
&=\frac{n!(r+j-1)!}{(r-1)!(n+j)!}.
\end{aligned}
$$

Here $B(a,b)=(a-1)!(b-1)!/(a+b-1)!$ for positive integers $a,b$; this identity also follows by repeated [integration by parts](../../../../../integration-by-parts.md). Taking $j=1,2$ yields

$$
\mathbb E[U_{(r)}]=\frac r{n+1},\qquad
\mathbb E[U_{(r)}^2]=\frac{r(r+1)}{(n+1)(n+2)}.
$$

Subtract the square of the first [moment](../../../../../moment.md) from the second to obtain the [variance](../../../../../variance-split.md):

$$
\boxed{\mathbb E[U_{(r)}]=\frac r{n+1},\qquad
\operatorname{Var}(U_{(r)})=
\frac{r(n-r+1)}{(n+1)^2(n+2)}.}
$$

These are exact finite-sample identities for each [uniform order statistic](../../../../../uniform-order-statistic.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
