<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $\phi(t)=t/(1+t)$. Every summand is nonnegative and at most $2^{-i}$, so the series defining $d$ converges and $d\leq1$. Symmetry follows from each $d_i$. If $d(x,y)=0$, every nonnegative summand is zero, hence every $d_i(x_i,y_i)=0$ and $x_i=y_i$. The converse is immediate.

For the [triangle inequality](../../../../../triangle-inequality.md), first observe that for $a,b\geq0$,

$$
\phi(a+b)=\frac a{1+a+b}+\frac b{1+a+b}\leq\frac a{1+a}+\frac b{1+b}=\phi(a)+\phi(b).
$$

Monotonicity of $\phi$ and the triangle inequality for $d_i$ therefore give

$$
\phi(d_i(x_i,z_i))\leq\phi(d_i(x_i,y_i))+\phi(d_i(y_i,z_i)).
$$

Multiply by $2^{-i}$ and sum the convergent nonnegative series. This proves the required triangle inequality for $d$, so **$d$ is a [metric](../../../../../metric.md)**. The construction combines a [bounded metric transform](../../../../../bounded-metric-transform.md) with a [countable product metric](../../../../../countable-product-metric.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
