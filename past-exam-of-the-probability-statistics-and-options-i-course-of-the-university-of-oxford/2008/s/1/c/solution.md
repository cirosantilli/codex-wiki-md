<h1 id="s/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [importance weight](../../../../../importance-weight.md) for the two normal densities is

$$
w_\sigma(x)=\frac1\sigma
\exp\left[\frac12(1-\sigma^{-2})x^2\right].
$$

Use $\hat\mu_N=N^{-1}\sum_iw_\sigma(X_i)f(X_i)$ with $X_i\sim N(0,1)$. Its second moment before averaging is

$$
E_q(w_\sigma^2f^2)=\frac1{\sigma^2\sqrt{2\pi}}
\int_{\mathbb R}f(x)^2
e^{-(\sigma^{-2}-1/2)x^2}\,dx.
$$

For the source's general assumption $E_pf^2<\infty$, a guaranteed range is

$$
\boxed{0<\sigma\leq1.}
$$

Indeed $w_\sigma\leq1/\sigma$ there, so $E_q(w_\sigma^2f^2)=E_p(w_\sigma f^2)\leq\sigma^{-1}E_pf^2<\infty$.

This range cannot be enlarged uniformly over all such $f$. If $\sigma>1$, choose $f^2=e^{ax^2}$ with

$$
\max(0,\sigma^{-2}-1/2)<a<\frac1{2\sigma^2}.
$$

Then $E_pf^2<\infty$ but the displayed weighted second-moment integral diverges. Thus no variance range depending only on $\sigma$ can characterize every individual integrand beyond the guaranteed range.

If an additional boundedness assumption on $f$ is intended, the familiar sufficient range becomes $0<\sigma<\sqrt2$. For $f=1$ this condition is also necessary, but a compactly supported $f$ can have finite weighted variance for every $\sigma$. Distinguishing these assumptions prevents imposing an unstated restriction on the source integrand.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [S](../../../s.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
