<h1 id="section-b/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\lambda=\ln(\rho^{-1})>0$. The [probability density function](../../../../../../probability-density-function.md) normalizes when $1=B\int_0^\infty e^{-\lambda x}dx=B/\lambda$, so $B=\lambda$. Its [survival function](../../../../../../survival-function.md) is $e^{-\lambda x}$ for $x\geq0$; hence, for $x>y\geq0$,

$$
\boxed{\mathbb P(X>x\mid X>y)=e^{-\lambda(x-y)}.}
$$

Differentiating this conditional tail gives

$$
\boxed{f_{X\mid X>y}(x)=\begin{cases}\lambda e^{-\lambda(x-y)},&x>y,\\0,&x<y.\end{cases}}
$$

The value assigned at the single endpoint does not affect any [probability](../../../../../../probability.md). The [memorylessness of the exponential distribution](../../../../../../memorylessness-of-the-exponential-distribution.md) says that $X-y$, conditional on $X>y$, is again an [exponential distribution](../../../../../../exponential-distribution.md) of rate $\lambda$. Its first two [moments](../../../../../../moment.md) are $1/\lambda$ and $2/\lambda^2$, found by [integration by parts](../../../../../../integration-by-parts.md), so translation leaves the [variance](../../../../../../variance-split.md) unchanged:

$$
\boxed{\operatorname{Var}(X\mid X>y)=\frac1{\lambda^2}=\frac1{[\ln(\rho^{-1})]^2}.}
$$

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
