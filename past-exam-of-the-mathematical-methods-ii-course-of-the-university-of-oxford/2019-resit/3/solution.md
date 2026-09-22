<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Assume $\lambda>0$, as required for normalization of the [exponential distribution](../../../exponential-distribution.md). Its [cumulative distribution function](../../../cumulative-distribution-function.md) is the integral of its [probability density function](../../../probability-density-function.md) from $-\infty$ to $x$:

$$
\boxed{F_X(x)=\begin{cases}0,&x<0,\\1-e^{-\lambda x},&x\geq0.\end{cases}}
$$

For the [expected value](../../../expected-value-split.md), [integration by parts](../../../integration-by-parts.md) gives

$$
\begin{aligned}
\mathbb E[X]
&=\int_0^\infty x\lambda e^{-\lambda x}\,dx\\
&=\left[-xe^{-\lambda x}\right]_0^\infty+\int_0^\infty e^{-\lambda x}\,dx
=\frac1\lambda.
\end{aligned}
$$

Similarly,

$$
\mathbb E[X^2]=\left[-x^2e^{-\lambda x}\right]_0^\infty
+2\int_0^\infty xe^{-\lambda x}\,dx=\frac2{\lambda^2}.
$$

The endpoint terms vanish because exponential decay dominates each fixed power of $x$. Therefore

$$
\boxed{\mathbb E[X]=\frac1\lambda,\qquad
\operatorname{Var}(X)=\mathbb E[X^2]-\mathbb E[X]^2=\frac1{\lambda^2}.}
$$

The mean has the same units as $X$, while the [variance](../../../variance-split.md) has their square; $\lambda$ has reciprocal units.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
