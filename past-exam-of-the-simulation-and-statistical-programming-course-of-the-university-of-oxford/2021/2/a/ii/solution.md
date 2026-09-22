<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Integrating the [conditional distribution](../../../../../conditional-distribution.md) against the [exponential distribution](../../../../../exponential-distribution.md) [probability density function](../../../../../probability-density-function.md) gives, for integer $k\geq0$,

$$
\begin{aligned}
\mathbb P(Y=k)
&=\int_0^\infty\frac{e^{-x}x^k}{k!}\lambda e^{-\lambda x}\,dx\\
&=\frac{\lambda}{k!}\frac{\Gamma(k+1)}{(1+\lambda)^{k+1}}
=\frac{\lambda}{1+\lambda}\left(\frac1{1+\lambda}\right)^k.
\end{aligned}
$$

Here the [gamma function](../../../../../gamma-function.md) identity $\Gamma(k+1)=k!$ evaluates the integral. Hence

$$
\boxed{Y\sim\operatorname{Geom}\!\left(\frac{\lambda}{1+\lambda}\right)}
$$

on $\{0,1,2,\ldots\}$. Put $r=1/(1+\lambda)$ and $\rho=1-r$. The [geometric series](../../../../../geometric-series.md) gives $F(k)=1-r^{k+1}$. Its generalized inverse, the [quantile function](../../../../../quantile-function.md), is

$$
\boxed{F^{-1}(u)=\left\lceil\frac{\log(1-u)}{\log r}\right\rceil-1,\qquad0<u<1.}
$$

This is the smallest nonnegative integer $k$ for which $1-r^{k+1}\geq u$; dividing by $\log r<0$ reverses the inequality. Draw $U$ from the [uniform distribution](../../../../../continuous-uniform-distribution.md) on $(0,1)$ and use this formula. The commonly used expression $\lfloor\log(1-U)/\log r\rfloor$ has the same [probability distribution](../../../../../probability-distribution-split.md), but differs from the exact generalized inverse when $U$ is precisely a jump value of the [cumulative distribution function](../../../../../cumulative-distribution-function.md). Such values have [probability](../../../../../probability.md) zero for an ideal continuous uniform draw.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
